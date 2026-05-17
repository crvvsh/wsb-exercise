# AI upośledza rozwój części programistów...

## Wstęp

_Wskazówka dla studentów: W tym miejscu wprowadźcie czytelnika w temat. Napiszcie, dlaczego integracja AI z systemami kontroli wersji (VCS) jest obecnie jednym z najważniejszych trendów w IT._

## 1. Agentic AI i inteligentna orkiestracja

**Agentic AI** to koncepcja, w której sztuczna inteligencja przestaje być tylko prostym asystentem, a staje się aktywnym uczestnikiem procesu deweloperskiego [1, 2]. Platformy takie jak GitLab Duo wykorzystują agenty AI do:

- **Automatycznej zamiany zgłoszeń (issues) w propozycje zmian (merge requests)** [2, 3].
- **Naprawiania luk w zabezpieczeniach** i przeprowadzania wstępnych recenzji kodu [3].
- Automatyzacji powtarzalnych zadań, przy jednoczesnym zachowaniu kontroli dewelopera nad procesem [3].

## 2. Ekosystem AI na platformie GitHub

GitHub rozwija szeroki wachlarz narzędzi wspieranych przez AI, które integrują się bezpośrednio z przepływem pracy programisty [4]. Do kluczowych rozwiązań należą:

- **GitHub Copilot:** Działający jako „AI pair programmer”, który sugeruje bloki kodu na podstawie komentarzy i istniejącej treści [5].
- **GitHub Spark:** Narzędzie do budowania i wdrażania inteligentnych aplikacji [4].
- **GitHub Models:** Platforma do zarządzania i porównywania promptów [4].
  Sztuczna inteligencja odpowiada już za niemal **40% kodu** w popularnych językach, takich jak Python, w plikach, gdzie Copilot jest włączony [6].

## 3. Kontrowersje prawne i kwestia własności intelektualnej

Rozwój narzędzi AI w ekosystemie Git nie odbywa się bez przeszkód. Największą kontrowersją jest **GitHub Copilot Litigation** – pozew zbiorowy dotyczący trenowania modeli na miliardach linii kodu open-source [7, 8]. Główne zarzuty to:

- **Naruszenie licencji open-source** poprzez ignorowanie warunków udostępniania kodu (np. braku podania autora) [7, 9].
- Wykorzystywanie kodu publicznego tak, jakby znajdował się w domenie publicznej [8].
- Ryzyko, że AI może sugerować duże fragmenty kodu objęte licencją bez powiadomienia o tym użytkownika [5].

## 4. Przyszłość kontroli wersji i Git 3.0

Przyszłość Gita to połączenie stabilności technicznej z nowymi standardami. Spodziewane wydanie **Git 3.0** (koniec 2026 r.) wprowadzi nazwę `main` jako domyślną oraz kontynuację migracji na bezpieczniejszy algorytm **SHA-256** [10, 11].

Wyzwania, przed którymi stoi ekosystem, to m.in.:

- **Skalowalność monorepozytoriów** i obsługa bardzo dużych plików [12].
- **Paradoks decentralizacji** – mimo rozproszonej natury Gita, rynek silnie koncentruje się wokół platformy GitHub należącej do Microsoftu [12].
- Pojawienie się nowej konkurencji w postaci systemów opartych na **blockchainie** [12, 13].

**Nadchodzące zmiany w Git 3.0***

Kluczowym celem przyszłej, dużej wersji systemu Git jest modernizacja i rozwiązanie problemów technicznych, które wynikają z kilkunastoletniego rozwoju poprzednich wydań.

* Algorytm SHA-256: Obecny standard SHA-1 staje się niewystarczający pod kątem bezpieczeństwa i rosnącej liczby projektów. Git 3.0 ma wprowadzić SHA-256 jako domyślny format dla nowych repozytoriów, eliminując ryzyko kolizji.

* Reftable zamiast plików tekstowych: Tradycyjny system przechowywania referencji oparty na plikach (ang. packed-refs) przy dużych bazach kodu działa wolno i ogranicza skalowalność. Format reftable przyspieszy operacje takie jak git fetch i git push.

* Wymagany Rust: Aby poprawić bezpieczeństwo pamięci i unowocześnić bazę projektu, kompilator języka Rust będzie wymagany do budowy Gita, co wyprze część kodu napisaną w C.

**Nowa gałąź domyślna**
W erze repozytoriów takich jak GitHub czy GitLab, używających gałęzi main, sam terminalowy Git zostanie wreszcie z nimi zsynchronizowany. Domyślną nazwą tworzoną przez polecenie git init będzie main zamiast dotychczasowego master.

**Wyzwania dla branży**
Głównym problemem wdrożenia zmian (zwłaszcza algorytmu SHA-256) nie jest sam program Git, ale całe powiązane środowisko. Platformy hostingowe i narzędzia CI/CD (GitHub, Bitbucket, narzędzia wspierające) będą musiały zaktualizować swoje systemy, aby obsłużyć nowy format.

**Nowe podejście do interfejsu i wygoda (Jujutsu / jj)**
Rozwój kontroli wersji nie kończy się na samym Gicie. W odpowiedzi na skomplikowaną obsługę niektórych poleceń (np. git rebase -i), coraz większą popularność zyskuje narzędzie Jujutsu (jj) od Google. Działa ono bezpośrednio na systemie Git (i używa jego silnika pod spodem), oferując przy tym od nowa przemyślane, znacznie bardziej intuicyjne środowisko.

**Ewolucja zorientowana na AI**
Generowanie kodu przez sztuczną inteligencję wyznacza kolejny wielki krok w ewolucji kontroli wersji. Tradycyjne przepływy pracy nie były projektowane na sytuację, w której asystenci AI generują tysiące linii kodu tygodniowo. Przyszłość to przejście na kontekstową kontrolę wersji, gdzie systemy będą automatycznie śledzić intencje stojące za zmianami, usprawniać asynchroniczne code review i inteligentnie scalać konflikty w czasie rzeczywistym.


## Podsumowanie :))

_Wskazówka: Podsumujcie zebrane informacje. Czy Waszym zdaniem AI zastąpi programistów, czy jedynie zmieni charakter ich pracy z systemem Git? [13, 14]_

---

### Bibliografia (Przykładowe źródła do uzupełnienia przez grupę)

- [4] About GitHub · GitHub.
- [1] Finally, AI for the entire software lifecycle, GitLab.
- [7] GitHub Copilot Intellectual Property Litigation.
- [11] Wszystkie notatki z 5/13/2026.
