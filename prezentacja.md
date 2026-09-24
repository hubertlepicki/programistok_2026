---
tytul: Inżynieria oprogramowania w dobie agentów AI
wydarzenie: Programistok 2026
prelegent: Hubert Łępicki
czas_minut: 30
---

# Inżynieria oprogramowania w dobie agentów AI

Każdy slajd ma trzy części:

- **Slajd**: to, co widzi sala.
- **Notatki**: krótkie punkty na telefon.
- **Tekst**: pełny tekst do wygłoszenia.

---

## 1. Inżynieria oprogramowania w dobie agentów AI

### Slajd

# Inżynieria oprogramowania w dobie agentów AI

Hubert Łępicki · Programistok 2026

### Notatki

- Przywitanie, podziękowanie organizatorom
- Kilka zdań o sobie [uzupełnić]
- Dwa pytania do sali: kto używał agenta? kto codziennie?

### Tekst

Dzień dobry! Bardzo się cieszę, że mogę być z Wami na Programistoku. Dziękuję organizatorom za zaproszenie, a Wam za to, że wybraliście tę salę.

Nazywam się Hubert Łępicki. [Dwa, trzy zdania o sobie.]

Na początek krótkie pytanie. Podnieście rękę, jeśli używaliście kiedyś agenta kodującego: Claude Code, Codexa, Cursora albo Copilota w trybie agenta. [Pauza.] A teraz ręka w górze, jeśli robicie to codziennie w pracy. [Pauza.] Dziękuję. Dlatego dziś nie będę mówił o tym, który agent jest najlepszy, tylko o tym, jak z nimi pracować, żeby powstawało dobre oprogramowanie.

---

## 2. Plan

### Slajd

- Skąd się wzięła inżynieria oprogramowania
- Praktyki i narzędzia z 60 lat, które dziś wracają
- Jak pracować z agentami, żeby powstawał dobry kod

> Agenci nie zastępują inżynierii oprogramowania.
> Sprawiają, że jest potrzebna bardziej niż kiedykolwiek.

### Notatki

- Część 1: historia, około 11 minut
- Część 2: agenci, około 16 minut
- Teza: przeczytać powoli

### Tekst

Plan jest taki. Przez pierwsze kilkanaście minut szybko przejdziemy przez historię: od programu Apollo, przez konferencje NATO, Uniksa, programowanie obiektowe i agile, aż po DevOps i GitHuba. Prawie każda dobra praktyka pracy z agentami, którą dziś odkrywamy, ma swój odpowiednik sprzed dwudziestu, czterdziestu albo sześćdziesięciu lat.

W drugiej, dłuższej części porozmawiamy o agentach: dlaczego szybkie generowanie kodu bez dyscypliny kończy się źle, co pomaga, jak dzielić pracę między wielu agentów, jak ich zabezpieczyć i jak przeglądać to, co wyprodukują.

Moja teza: agenci nie zastępują inżynierii oprogramowania. Sprawiają, że jest potrzebna bardziej niż kiedykolwiek.

---

## 3. Margaret Hamilton i program Apollo

### Slajd

- MIT Instrumentation Lab: oprogramowanie lotu Apollo
- Około 36 tys. słów pamięci stałej i 2 tys. roboczej
- Pamięć linowa (core rope): program ręcznie przewlekany drutem, zamrażany miesiące przed startem
- Połowa lat 60.: opóźnienia, brak pamięci, interwencja NASA
- „Software engineering”: żeby oprogramowanie traktowano jak inżynierię

### Notatki

- Hamilton kierowała zespołem oprogramowania lotu (moduł dowodzenia i lądownik)
- Bill Tindall z NASA porządkuje projekt, 1966–67
- Termin: najpierw żart, potem wymusza szacunek dla oprogramowania

### Tekst

Zaczynamy w latach sześćdziesiątych, od Margaret Hamilton. Kierowała w laboratorium MIT zespołem, który pisał oprogramowanie lotu dla programu Apollo.

Komputer pokładowy miał około trzydziestu sześciu tysięcy słów pamięci stałej i dwóch tysięcy słów pamięci roboczej. Program zapisywano w pamięci linowej (core rope): pracownice fabryki ręcznie przewlekały druty przez rdzenie magnetyczne. Trwało to tygodnie, więc program zamrażano na miesiące przed startem. Potem nie było już poprawek.

W połowie dekady oprogramowanie się spóźniało i nie mieściło w pamięci. NASA wysłała do MIT swojego inżyniera, Billa Tindalla, żeby zaprowadził porządek.

Właśnie wtedy Hamilton zaczęła nazywać swoją pracę inżynierią oprogramowania (software engineering). Na początku się z tego śmiano. Ona chciała, żeby oprogramowanie traktowano tak poważnie jak sprzęt, bo od niego zależało życie astronautów.

---

## 4. Jak pracował zespół Apollo

### Slajd

- Symulatory cyfrowe (na komputerach mainframe) i hybrydowe (z prawdziwym komputerem pokładowym)
- Kilka poziomów testów, aż po pełne próby misji z astronautami
- Czytanie wydruków kodu w zespole, kontrola zmian, zamrażanie wersji
- Projektowanie na błąd człowieka
- Priorytety zadań i restart bez utraty stanu
- Apollo 11: alarmy 1201 i 1202, a lądowanie trwa dalej

### Notatki

- Córka Hamilton uruchamia P01 w trakcie lotu; „astronauta tego nie zrobi”
- Apollo 8: Lovell robi to samo, procedura naprawcza gotowa
- Zapowiedź: symulator, testy, kontrola zmian, błąd człowieka → wrócą przy agentach

### Tekst

Jak ten zespół pracował? Programu nie dało się przetestować w kosmosie, więc testowano go w symulacji. Były symulatory cyfrowe na dużych komputerach i symulatory hybrydowe, w których prawdziwy komputer pokładowy pracował w symulowanym otoczeniu. Testy miały kilka poziomów, aż po pełne próby misji z astronautami. Wydruki kodu czytano wspólnie, a zmiany przechodziły przez komisję.

Najważniejsze było jednak założenie, że błędy się zdarzą. Córka Hamilton, bawiąc się symulatorem, uruchomiła w trakcie lotu program przedstartowy i skasowała dane nawigacyjne. Hamilton usłyszała, że astronauta nigdy tego nie zrobi. W czasie misji Apollo 8 Jim Lovell zrobił dokładnie to, a zespół miał gotową procedurę naprawczą.

Podczas lądowania Apollo 11 komputer był przeciążony i zgłaszał alarmy 1201 i 1202. Dzięki priorytetom zadań i restartom bez utraty stanu utrzymał to, co najważniejsze. Do każdej z tych praktyk wrócimy przy agentach.

---

## 5. NATO 1968: dyscyplina dostaje nazwę

### Slajd

- Garmisch 1968, Rzym 1969: Komitet Naukowy NATO
- Dlaczego NATO? Sputnik, obronność zależna od oprogramowania, luka technologiczna Europa–USA
- Kryzys oprogramowania (software crisis): projekty spóźnione, drogie, zawodne
- Nazwa wybrana celowo, jako prowokacja
- Efekt: czasopismo, konferencja ICSE, przedmioty na uczelniach

### Notatki

- Około 50 osób z uczelni i przemysłu, przewodniczył Friedrich L. Bauer, raport: Naur i Randell
- Konferencje cywilne, raporty jawne
- OS/360 IBM jako symbol kryzysu
- Rzym 1969: spór teoretyków z praktykami

### Tekst

Termin rozpowszechniła instytucja, której mało kto by się tu spodziewał: NATO. W 1968 roku w Garmisch i rok później w Rzymie Komitet Naukowy NATO zorganizował konferencje o inżynierii oprogramowania.

Dlaczego NATO? Po Sputniku sojusz uznał, że musi wzmacniać zachodnią naukę, i powołał Komitet Naukowy. Pod koniec lat sześćdziesiątych obrona powietrzna, wczesne ostrzeganie i dowodzenie zależały od coraz większych programów, które były spóźnione, drogie i zawodne. W przemyśle było tak samo, a symbolem stał się system OS/360 firmy IBM. Mówiono o kryzysie oprogramowania (software crisis). Do tego Europa bała się, że zostaje w tyle za Ameryką.

Nazwę wybrano celowo, jako prowokację: ta dziedzina jeszcze nie jest inżynierią, ale powinna nią być. Efekt? Po kilku latach istniały już czasopismo, konferencja ICSE i przedmioty na uczelniach. Dyscyplina dostała nazwę i program.

---

## 6. Wojsko i administracja formalizują proces

### Slajd

- **Zamawianie**: kontrakty z fazami i dokumentami do odbioru
- **Projektowanie**: formalne przeglądy wymagań i projektu
- **Wycena**: modele kosztów (COCOMO), punkty funkcyjne
- **Wytwarzanie**: normy Departamentu Obrony, język Ada
- **Ocena dostawców**: SEI i model dojrzałości CMM
- Model kaskadowy (waterfall) wpisany w umowy

### Notatki

- Benington 1956 (SAGE): fazy; Royce 1970 (TRW): ostrzegał przed jednokierunkowością
- Normy: MIL-STD-1679 (1978), DOD-STD-2167 (1985)
- Przeglądy: SRR, PDR, CDR
- Zyski: przewidywalność, odpowiedzialność; koszty: późna zmiana droga, testy na końcu
- Zapowiedź: wróci przy „specyfikacja → kod”

### Tekst

Przez kolejne dekady największym zamawiającym oprogramowanie były wojsko i administracja. To one sformalizowały, jak się oprogramowanie zamawia, wycenia, projektuje i odbiera.

Już w 1956 roku Herbert Benington opisał fazy budowy systemu obrony powietrznej SAGE. W 1970 roku Winston Royce z firmy zbrojeniowej TRW opisał to, co później nazwano modelem kaskadowym (waterfall), choć sam ostrzegał przed czysto jednokierunkowym przebiegiem.

Umowy wymagały faz, dokumentów i formalnych przeglądów wymagań i projektu. Normy Departamentu Obrony opisywały, co ma powstać w każdej fazie. Do wyceny powstały modele kosztów, na przykład COCOMO Barry'ego Boehma. Pentagon sfinansował Software Engineering Institute, który stworzył model dojrzałości CMM do oceny dostawców.

To dało przewidywalność i jasną odpowiedzialność. Późna zmiana wymagań była jednak bardzo droga, a testy przychodziły na końcu. Wrócimy do tego przy generowaniu kodu ze specyfikacji.

---

## 7. Lata 60. i 70.: narzędzia, których agenci używają do dziś

### Slajd

- Podział czasu (time-sharing, CTSS 1961), maszyny wirtualne (IBM CP-67, 1967)
- Unix (1969), C (1972), potoki (pipes, 1973), powłoka i skrypty
- diff (1974), później patch (1985)
- make (1976), SCCS (1972), lint (1978)
- chroot (1979): przodek kontenerów
- Zasada najmniejszych uprawnień (least privilege, Saltzer i Schroeder, 1975)

### Notatki

- Filozofia Uniksa (McIlroy): małe programy, jedna rzecz, tekst jako interfejs
- Agent = program w powłoce: grep, git, testy; zmiany jako diff
- CP-67 → izolacja agentów w maszynach wirtualnych
- Saltzer i Schroeder: każdy program ma tylko uprawnienia potrzebne do swojej pracy

### Tekst

Teraz kilka wynalazków, z których agenci korzystają dosłownie.

Systemy z podziałem czasu (time-sharing), jak CTSS z 1961 roku, pozwoliły wielu osobom pracować na jednym komputerze jednocześnie. W 1967 roku IBM uruchomił CP-67: każdy użytkownik dostawał własną, izolowaną maszynę wirtualną.

Potem przyszły Unix i język C. Doug McIlroy wymyślił potoki (pipes) i opisał filozofię Uniksa: małe programy, które robią jedną rzecz dobrze i komunikują się tekstem. Do tego doszły powłoka i skrypty, diff do porównywania wersji, później patch do nakładania zmian, make do budowania, SCCS do kontroli wersji i lint do wyłapywania podejrzanego kodu. W 1979 roku pojawił się chroot, przodek kontenerów. A w 1975 roku Saltzer i Schroeder opisali zasadę najmniejszych uprawnień (least privilege).

Agent kodujący to w praktyce program, który pracuje w powłoce, używa grepa, gita i testów, a swoje zmiany pokazuje jako diff. Tekstowy interfejs Uniksa okazał się idealny dla modeli językowych.

---

## 8. Lata 80. i 90.: obiekty, modele, generatory kodu

### Slajd

- Smalltalk-80: obiekty, żywe środowisko, automatyczna refaktoryzacja, SUnit
- C++, Eiffel (projektowanie przez kontrakt)
- Wzorce projektowe (1994), refaktoryzacja (Fowler, 1999)
- UML (1997)
- Narzędzia CASE: kod generowany z diagramów, obietnice większe niż efekty
- Brooks, *No Silver Bullet* (1986): złożoność istotna i przypadkowa

### Notatki

- Ze społeczności Smalltalka: wzorce, pierwsza wiki, XP, rodzina xUnit
- CASE: próba „specyfikacja → kod”, wróci przy Symphony
- Brooks: rama dla całej części o agentach

### Tekst

Lata osiemdziesiąte i dziewięćdziesiąte to programowanie obiektowe. Smalltalk z Xerox PARC dał obiekty i żywe środowisko programistyczne, a później pierwsze narzędzie do automatycznej refaktoryzacji i framework testów SUnit. Ze społeczności Smalltalka wyszły też wzorce, pierwsza wiki i programowanie ekstremalne.

Przyszły C++, Eiffel z projektowaniem przez kontrakt, katalog wzorców projektowych, książka Fowlera o refaktoryzacji, a w 1997 roku UML. Narzędzia CASE obiecywały, że kod będzie generowany z diagramów. Obietnice były dużo większe niż efekty.

W 1986 roku Fred Brooks napisał esej *No Silver Bullet*. Oddzielił w nim złożoność przypadkową, wynikającą z narzędzi, od złożoności istotnej, wynikającej z samego problemu. Napisał, że żadna pojedyncza technologia nie da dziesięciokrotnej poprawy. Warto to pamiętać, gdy ktoś obiecuje, że AI napisze za nas cały system.

---

## 9. Agile: XP, TDD i BDD

### Slajd

- Manifest Agile (2001)
- Programowanie ekstremalne (Extreme Programming): pary, ciągła integracja, małe wydania, refaktoryzacja
- TDD: czerwony → zielony → refaktoryzacja (red → green → refactor)
- BDD: zachowanie opisane przykładami
  - Zakładając… / Gdy… / Wtedy… (Given / When / Then)

> „Nie jestem świetnym programistą. Jestem dobrym programistą ze świetnymi nawykami.” (Kent Beck)

### Notatki

- TDD: zobacz czerwony test i sprawdź, że pada z właściwego powodu
- Test, który przechodzi od razu, niczego nie dowodzi
- BDD: Dan North, 2006; Cucumber i Gherkin: scenariusze czytelne dla biznesu
- Cytat Becka: wrócę do niego przy agentach

### Tekst

W 2001 roku siedemnaście osób napisało Manifest Agile. Ważniejsze od nazwy były jednak praktyki, zwłaszcza z programowania ekstremalnego (Extreme Programming) Kenta Becka: programowanie w parach, ciągła integracja, małe wydania i ciągła refaktoryzacja.

Dla nas najważniejsze jest TDD, czyli programowanie sterowane testami (test-driven development). Najpierw piszesz mały test, który nie przechodzi: czerwony. Potem najmniej kodu, żeby przeszedł: zielony. Potem porządkujesz kod przy zielonych testach: refaktoryzacja. I od nowa. Ważny szczegół: czerwony test trzeba zobaczyć i sprawdzić, że pada z właściwego powodu. Test, który przechodzi od razu, niczego nie dowodzi.

Kilka lat później Dan North zaproponował BDD, czyli zachowanie systemu opisane przykładami: zakładając, że…, gdy…, wtedy… Takie scenariusze mogą czytać ludzie z biznesu, a uruchamiać komputer.

Kent Beck mówił o sobie, że nie jest świetnym programistą, tylko dobrym programistą ze świetnymi nawykami. Zapamiętajcie to zdanie.

---

## 10. DevOps, infrastruktura jako kod, kontenery

### Slajd

- DevOps (2009): jeden zespół od kodu do produkcji
- Potok wdrożeniowy (deployment pipeline), ciągłe dostarczanie (continuous delivery)
- Infrastruktura jako kod (Infrastructure as Code): Puppet, Chef, Ansible, Terraform
- Kontenery: Docker (2013), Kubernetes (2014)
- Sekrety poza repozytorium, menedżery sekretów, najmniejsze uprawnienia w praktyce

### Notatki

- chroot 1979 → kontenery
- Menedżer sekretów: dostęp na określony czas i zakres
- Dla agentów: powtarzalne, izolowane środowisko w minutę

### Tekst

Pod koniec pierwszej dekady XXI wieku powstał ruch DevOps: jeden zespół odpowiada za oprogramowanie od napisania do działania na produkcji. Pojawił się potok wdrożeniowy (deployment pipeline): każda zmiana automatycznie przechodzi przez budowanie, testy i wdrożenie.

Konfigurację serwerów zaczęto zapisywać jako kod. To infrastruktura jako kod (Infrastructure as Code): Puppet, Chef, Ansible, Terraform. Docker spakował aplikację razem ze środowiskiem, a Kubernetes zaczął zarządzać tysiącami kontenerów.

Dojrzało też podejście do sekretów. Hasła i klucze nie trafiają do repozytorium, tylko do menedżerów sekretów, które wydają je na określony czas i w określonym zakresie. Zasada najmniejszych uprawnień stała się codzienną praktyką.

Dla agentów to fundament. W minutę stawiamy powtarzalne, izolowane środowisko i dajemy agentowi dokładnie te uprawnienia, których potrzebuje.

---

## 11. Git, pull requesty, testy, dane

### Slajd

- Git (2005), GitHub (2008): tanie gałęzie, pull requesty
- Przegląd kodu (code review) jako codzienna praktyka
- Piramida testów: dużo szybkich, mało wolnych
- DORA, *Accelerate* (2018): małe zmiany, często → szybciej **i** stabilniej

### Notatki

- Inspekcje Fagana (IBM, 1976) → pull requesty
- Cztery miary DORA: częstotliwość wdrożeń, czas od zmiany do produkcji, odsetek zmian powodujących awarię, czas przywrócenia usługi
- Przejście: „Tyle historii”

### Tekst

Ostatni przystanek historyczny. W 2005 roku powstał Git, a w 2008 roku GitHub z pull requestami, czyli propozycjami zmian z dyskusją i przeglądem w jednym miejscu. Przegląd kodu (code review), który w latach siedemdziesiątych był formalną inspekcją w IBM, stał się codziennością. Upowszechniła się piramida testów: dużo szybkich testów jednostkowych, mniej integracyjnych, niewiele wolnych testów przez interfejs.

W 2018 roku autorzy badań DORA pokazali w książce *Accelerate*, na danych od dziesiątek tysięcy osób, że najlepsze zespoły wdrażają małe zmiany często i mają przy tym mniej awarii. Szybkość i stabilność nie są w konflikcie. Warunek to małe partie, automatyczne testy i szybka informacja zwrotna.

Tyle historii. Przejdźmy do agentów.

---

## 12. Od podpowiedzi do agentów

### Slajd

- 2021: podpowiadanie kodu
- 2022: rozmowa z modelem
- 2025: agenci (Claude Code, Codex, Gemini CLI, Cursor…)
- Agent = pętla: model proponuje działanie → narzędzie je wykonuje → wynik wraca do modelu
- Standardy: MCP, AGENTS.md, umiejętności (skills)
- Brooks: mniej złożoności przypadkowej, tyle samo istotnej

### Notatki

- Copilot 2021–22, ChatGPT listopad 2022, MCP listopad 2024, Claude Code i Codex 2025
- Wąskie gardło: z pisania kodu na specyfikację i weryfikację

### Tekst

W ciągu pięciu lat przeszliśmy trzy etapy. W 2021 roku narzędzia podpowiadały kolejne wiersze. Pod koniec 2022 roku zaczęliśmy z modelami rozmawiać. Od 2025 roku na dobre pracujemy z agentami.

Agent to prosta pętla: model proponuje działanie (przeczytaj plik, zmień plik, uruchom testy), program je wykonuje, a wynik wraca do modelu. I tak do skutku. Powstały też pierwsze standardy: MCP do podłączania narzędzi, AGENTS.md z instrukcjami w repozytorium i umiejętności (skills) do powtarzalnych zadań.

Wróćmy do Brooksa. Agent świetnie zmniejsza złożoność przypadkową: szablonowy kod, szukanie w dokumentacji, pamiętanie API. Nie usuwa złożoności istotnej. Nadal ktoś musi zdecydować, co system ma robić, i sprawdzić, czy to robi. Wąskie gardło przesuwa się z pisania kodu na specyfikację i weryfikację.

---

## 13. Programowanie na wyczucie (vibe coding)

### Slajd

- „Vibe coding” (Karpathy, luty 2025): opisuję, akceptuję, nie czytam kodu
- Szybko powstaje dużo kodu, często niskiej jakości (slop)
- Duplikacja, brak testów, niespójność, kod, którego nikt nie rozumie
- To nie jest nowy problem: tak pracuje człowiek bez dobrych praktyk
- Agent robi to po prostu 10 razy szybciej

### Notatki

- Do prototypów dobre, do systemów utrzymywanych latami złe
- METR 2025: 16 doświadczonych programistów, 19% wolniej, a wrażenie: 20% szybciej
- DORA 2025: AI wzmacnia to, co już jest w zespole

### Tekst

W lutym 2025 roku Andrej Karpathy nazwał nowy styl pracy: vibe coding, czyli programowanie na wyczucie. Opisujesz, czego chcesz, akceptujesz wszystko, co zaproponuje agent, i nie czytasz kodu. Do weekendowego prototypu to świetne.

Kłopot zaczyna się, gdy tak powstaje system, który ma żyć latami. Powstaje wtedy szybko dużo kodu niskiej jakości: zduplikowanego, bez testów, niespójnego, niezrozumiałego dla zespołu. Po angielsku mówi się na to slop.

To jednak nie jest nowy problem. Tak wygląda kod człowieka, który nie stosuje dobrych praktyk: nie pisze testów, nie refaktoryzuje, nie daje nikomu kodu do przeglądu. Agent robi to po prostu dziesięć razy szybciej.

W badaniu METR z 2025 roku doświadczeni programiści z narzędziami AI byli o 19 procent wolniejsi, choć byli przekonani, że pracowali o 20 procent szybciej. Raporty DORA opisują AI jako wzmacniacz: wzmacnia i dobre, i złe praktyki zespołu.

---

## 14. Ograniczenia modeli

### Slajd

- Ograniczony kontekst: widzi tylko część projektu, nie pamięta poprzednich sesji
- W długiej sesji gubi wątek i zapomina wcześniejsze ustalenia
- Streszczanie kontekstu (compaction) gubi szczegóły
- Luki w wymaganiach wypełnia pewnie i wiarygodnie
- Czasem wymyśla API i pakiety
- „Gotowe” od agenta to jeszcze nie dowód

### Notatki

- *Lost in the Middle* (2023): najsłabiej wykorzystany jest środek kontekstu
- Człowiek też ma ograniczoną pamięć roboczą → praktyki dają zewnętrzną strukturę

### Tekst

Skąd to się bierze? Modele mają konkretne ograniczenia.

Po pierwsze, ograniczony kontekst. Model widzi tylko część projektu i nie pamięta poprzednich sesji. Po drugie, w długiej sesji gubi wątek. Badania pokazują, że im dłuższy kontekst, tym gorzej model korzysta z informacji ze środka. Gdy kontekst się zapełnia, jest streszczany i szczegóły giną. Agent zapomina, co ustaliliście godzinę temu.

Po trzecie, luki w wymaganiach wypełnia pewnie i wiarygodnie. Nie zapyta, jeśli go do tego nie skłonimy. Potrafi też wymyślić metodę API albo pakiet, które nie istnieją. Po czwarte, gdy agent mówi „gotowe”, to jeszcze nie jest dowód, że działa.

Człowiek też ma ograniczoną pamięć roboczą i też się myli. Dlatego wymyśliliśmy praktyki, które dają zewnętrzną strukturę. Agent potrzebuje ich jeszcze bardziej.

---

## 15. TDD jako struktura dla agenta

### Slajd

- Jedno zachowanie na raz: mały krok mieści się w kontekście
- **Czerwony**: test przed kodem, uruchomiony, pada z oczekiwanym komunikatem
- **Zielony**: najmniej kodu, żeby przeszedł
- **Refaktoryzacja**: porządek przy zielonych testach
- Testy to pamięć projektu, której agent nie zgubi
- Zakaz fałszywej zieleni: nie usuwamy, nie pomijamy, nie osłabiamy testów

### Notatki

- Test po kodzie od tego samego agenta często utrwala błąd
- Czerwony z właściwym komunikatem = test naprawdę coś sprawdza
- Reguła „nie osłabiamy testów” w instrukcjach i w przeglądzie

### Tekst

I tu dochodzimy do sedna. Moim zdaniem TDD to najlepsze, co możemy dać agentowi.

Po pierwsze, TDD wymusza małe kroki: jedno zachowanie, jeden test, jedna zmiana. Taki krok mieści się w kontekście modelu i łatwo go przejrzeć.

Po drugie, test napisany przed kodem jest niezależnym opisem tego, co ma się stać. Jeśli agent najpierw napisze kod, a potem test, test często utrwala błąd, bo opisuje to, co kod robi, a nie to, co powinien. Dlatego każę agentowi uruchomić nowy test i pokazać, że pada z oczekiwanym komunikatem. Dopiero wtedy wiem, że test coś sprawdza.

Po trzecie, testy są pamięcią projektu. Agent zapomni, co ustaliliśmy rano. Test nie zapomni.

Jest też pułapka. Agent, któremu każe się doprowadzić testy do zieleni, potrafi osłabić asercję albo pominąć test. Potrzebna jest twarda reguła: nie usuwamy, nie pomijamy i nie osłabiamy testów, żeby przeszły.

---

## 16. Najpierw przykłady i pytania, potem kod

### Slajd

- Wymagania jako przykłady (BDD):
  - *Zakładając*, że bilet został już użyty,
  - *gdy* ktoś zeskanuje go przy wejściu,
  - *wtedy* bramka się nie otwiera, a obsługa widzi, kiedy bilet użyto
- Przykład → test akceptacyjny → najpierw czerwony → z zewnątrz do środka (outside-in)
- Agent pyta o niejasności, zamiast zgadywać
- Plan przed zmianą; ustalamy, co znaczy „gotowe”
- Najpierw szkielet (walking skeleton)

### Notatki

- Tryb planowania w agentach
- Outside-in: Freeman i Pryce, *Growing Object-Oriented Software, Guided by Tests* (2009)
- Szkielet: najcieńszy działający przekrój przez cały system

### Tekst

Druga rzecz: zanim agent napisze kod, ustalmy, co znaczy „gotowe”. Najlepiej przykładami, w stylu BDD. Zamiast „obsłuż wykorzystane bilety” piszemy: zakładając, że bilet został już użyty, gdy ktoś zeskanuje go przy wejściu, wtedy bramka się nie otwiera, a obsługa widzi, kiedy bilet użyto. Taki przykład od razu staje się testem akceptacyjnym. Piszemy go najpierw, patrzymy, jak pada, i schodzimy do testów jednostkowych, z zewnątrz do środka.

Agent powinien też pytać, zamiast zgadywać. Większość agentów ma tryb planowania: najpierw plan i rozmowa, potem akceptacja, a dopiero potem zmiany. Warto też zacząć od szkieletu (walking skeleton), czyli najcieńszego działającego przekroju przez cały system, zanim agent zacznie rozbudowywać szczegóły.

---

## 17. Pętla jakości

### Slajd

1. Refaktoryzacja w każdym cyklu, także testów
2. Przegląd wewnętrzny: drugi agent z czystym kontekstem
3. Zgodność z wymaganiami: to, o co proszono, i nic więcej
4. Standardy zespołu (guidelines, stylebook) dostępne dla agenta

Typowe wady kodu agentów: rozszerzanie zakresu, duplikacja zamiast użycia istniejącego kodu, nadmiarowa obrona, komentarze opisujące kod

### Notatki

- Reguły Becka: przechodzi testy, wyraża intencję, bez duplikacji, najmniej elementów
- Recenzent z czystym kontekstem nie zna uzasadnień autora
- Usuwanie kodu jest dziś tanie: robić to regularnie

### Tekst

Zielone testy to nie koniec. Po każdym cyklu przychodzi refaktoryzacja, i to nie tylko kodu, ale też testów. Agent w trakcie pracy tworzy sporo testów pomocniczych, które potem warto scalić albo usunąć.

Potem przegląd wewnętrzny. Dobrze działa drugi agent z czystym kontekstem, który nie zna uzasadnień autora i widzi tylko diff i wymagania.

Trzecie sprawdzenie: czy zmiana robi to, o co proszono, i nic więcej. Agenci lubią dodawać rzeczy przy okazji: opcje, abstrakcje na zapas, obsługę przypadków, które nie mogą wystąpić, komentarze opisujące kod.

Czwarte to standardy zespołu. Jeśli macie wytyczne (guidelines) albo księgę stylu (stylebook), zapiszcie je tak, żeby agent mógł je wczytać.

I dobra wiadomość: refaktoryzacja i usuwanie kodu nigdy nie były tak tanie. Korzystajcie z tego regularnie.

---

## 18. Agent sam klika po aplikacji

### Slajd

- Agent uruchamia aplikację i przechodzi ścieżkę użytkownika w przeglądarce
- Playwright, Chrome DevTools, podłączone przez MCP
- Zrzuty ekranu, konsola, ruch sieciowy, logi serwera
- Widzi to, czego nie widzą testy jednostkowe: układ, komunikaty, urwane przepływy
- Jak w Apollo: najpierw misja w symulatorze

### Notatki

- Środowisko dla zadania: własne porty, baza, dane testowe
- Zrzuty i nagranie jako dowód wykonania
- Człowiek i tak patrzy na wynik

### Tekst

Człowiek, zanim powie, że skończył, zwykle uruchamia aplikację i się przez nią przeklikuje. Agent może zrobić to samo. Przez Playwrighta albo Chrome DevTools, podłączone przez MCP, otwiera przeglądarkę, loguje się, przechodzi ścieżkę użytkownika, robi zrzuty ekranu, czyta konsolę, ruch sieciowy i logi serwera.

Dzięki temu wyłapuje to, czego testy jednostkowe nie widzą: rozjechany układ, zły komunikat, przycisk, który nic nie robi, przepływ, który się urywa.

To ta sama idea co w Apollo: zanim polecisz, przeleć misję w symulatorze. Zrzuty ekranu albo nagranie zostają jako dowód wykonania dla człowieka, który przegląda zmianę.

---

## 19. Kontekst to też kod projektu

### Slajd

- AGENTS.md jako spis treści, a nie encyklopedia
- Umiejętności (skills): jak uruchomić testy, jak zrobić przegląd, jak przygotować commit
- Instrukcje się starzeją: przeglądamy je jak kod
- Reguła od miękkiej do twardej:
  - uwaga w przeglądzie → dokument → umiejętność → linter / test / hook
- Komunikat lintera jako instrukcja dla agenta

### Notatki

- OpenAI, *harness engineering* (luty 2026): duży plik instrukcji zawiódł (kontekst, rozmycie reguł, starzenie się); zastąpił go spis treści około 100 wierszy
- Hook jest deterministyczny: model go nie obejdzie
- Parnas: moduł, który da się zrozumieć bez reszty systemu, mieści się w kontekście

### Tekst

Agent zaczyna każdą sesję bez pamięci o projekcie. Wszystko, co powinien wiedzieć, musi być zapisane w repozytorium. Standardem stał się plik AGENTS.md. W lutym 2026 roku OpenAI opisało, że ich duży plik instrukcji zawiódł: nie mieścił się w kontekście, rozmywał najważniejsze reguły i szybko się starzał. Zastąpili go krótkim spisem treści, który odsyła do szczegółowych dokumentów.

Szczegóły warto pakować w umiejętności, które agent wczytuje dopiero wtedy, gdy są potrzebne.

Najważniejsza zasada: ważna reguła powinna przechodzić od formy miękkiej do twardej. Najpierw uwaga w przeglądzie, potem zdanie w dokumentacji, potem umiejętność, a na końcu linter, test albo hook, którego agent nie obejdzie. I jeszcze jedno: komunikat lintera piszcie jak instrukcję. Nie tylko co jest źle, ale też co zrobić zamiast tego.

---

## 20. Wiele zadań naraz

### Slajd

- Drzewa robocze gita (git worktree): wiele gałęzi z jednego repozytorium
- Worktree izoluje tylko pliki → kontener albo maszyna wirtualna dla każdego zadania
- Zadania muszą być niezależne: granice modułów decydują (prawo Conwaya)
- Limit wyznacza uwaga człowieka, nie liczba agentów
- Koszt: tokeny i czas przeglądu

### Notatki

- Podział czasu 1961, CP-67 1967 → wielu agentów na jednej maszynie
- Osobne porty, baza danych, dane testowe dla każdego zadania
- Prawo Brooksa: koordynacja nie znika
- Tylu agentów, ile wyników jesteś w stanie ocenić

### Tekst

Agenci pozwalają pracować nad wieloma zadaniami naraz. Najprostsze narzędzie to drzewa robocze gita (worktrees): kilka katalogów z jednego repozytorium, każdy na innej gałęzi, w każdym inny agent.

Worktree izoluje jednak tylko pliki. Jeśli aplikacja potrzebuje bazy danych i usług na konkretnych portach, agenci zaczną sobie przeszkadzać. Wtedy każde zadanie potrzebuje własnego kontenera albo maszyny wirtualnej. To ten sam pomysł, który IBM zrealizował w 1967 roku.

Dwie rzeczy są ważne. Po pierwsze, zadania muszą być naprawdę niezależne. Jeśli dwa zmieniają ten sam moduł, będą konflikty albo dwa różne rozwiązania tego samego problemu. Działa tu prawo Conwaya: podział pracy musi pasować do podziału systemu.

Po drugie, limit wyznacza człowiek. Każdy wynik trzeba przejrzeć i zintegrować. Uruchamiajcie tylu agentów, ile wyników jesteście w stanie rzetelnie ocenić.

---

## 21. Izolacja i najmniejsze uprawnienia, ale z dostępem do wiedzy

### Slajd

**Izolacja**

- Osobne środowisko dla każdego projektu: pliki, sekrety, sieć
- Bez produkcji i produkcyjnych danych; sekrety z menedżera
- Działania nieodwracalne (commit, push, usuwanie, publikacja) tylko za zgodą

**Dostęp do wiedzy**

- Zgłoszenia, dokumentacja, system projektowy (np. Figma) przez MCP
- Tylko do odczytu, wąski zakres, osobne konto dla agenta

**Treść z zewnątrz to dane, nie polecenia** (prompt injection)

### Notatki

- Saltzer i Schroeder, 1975
- Agent bez kontekstu zgaduje; agent z pełnym dostępem jest ryzykiem
- Zmyślone nazwy pakietów rejestrowane złośliwie → nowe zależności zatwierdza człowiek
- Krótkotrwałe tokeny, dziennik działań

### Tekst

Bezpieczeństwo. Tu ścierają się dwie potrzeby.

Pierwsza to izolacja. Każdy projekt powinien mieć osobne środowisko: własne pliki, własne sekrety, ograniczoną sieć. Agent pracujący nad jednym projektem nie powinien widzieć kluczy innego. Obowiązuje zasada najmniejszych uprawnień: żadnej produkcji, żadnych produkcyjnych danych, sekrety z menedżera, a nie z pliku. Działania trudne do cofnięcia, czyli commit, push, usuwanie i publikowanie, tylko za zgodą człowieka.

Druga potrzeba: agent bez kontekstu zgaduje. Potrzebuje dostępu do wiedzy: zgłoszeń, dokumentacji, systemu projektowego, na przykład Figmy. MCP pozwala to podłączyć, najlepiej tylko do odczytu, z wąskim zakresem i osobnym kontem dla agenta.

I jeszcze jedno: treść z zewnątrz to dane, a nie polecenia. Opis zgłoszenia czy komentarz w PR mogą zawierać tekst, który próbuje przejąć sterowanie agentem. To wstrzykiwanie poleceń (prompt injection).

---

## 22. Pull requesty, które da się przejrzeć

### Slajd

- Jeden PR, jeden cel, jedna decyzja
- Najpierw refaktoryzacja bez zmiany zachowania, potem zmiana zachowania
- Stos zależnych PR-ów (stacked PRs): każdy buduje na poprzednim
- Opis: co, dlaczego, jak sprawdzone
- Utrzymanie stosu (rebase, poprawki w środku) to dla agenta tania praca

### Notatki

- Duży diff w godzinę = dzień przeglądu albo przegląd pobieżny
- Stacked diffs: Phabricator w Facebooku; dziś Graphite, Sapling, `git rebase --update-refs`
- DORA: małe partie

### Tekst

Agent w godzinę może wygenerować zmianę, której przegląd zajmie człowiekowi dzień. Albo, co gorsze, zmiana zostanie przejrzana pobieżnie. Dlatego pull requesty trzeba projektować z myślą o przeglądzie.

Jedna zmiana, jeden cel. Jeśli nowa funkcja wymaga refaktoryzacji, najpierw osobny PR z refaktoryzacją bez zmiany zachowania, a potem PR ze zmianą zachowania.

Większą pracę układamy w stos zależnych PR-ów (stacked PRs): każdy buduje na poprzednim i każdy da się przejrzeć osobno. Ta praktyka wyrosła w Facebooku, a dziś wspierają ją narzędzia takie jak Graphite czy Sapling, a nawet sam git. Kiedyś największym kosztem stosu było jego utrzymanie: rebase, poprawki w środku stosu. Dla agenta to tania, mechaniczna praca.

W opisie PR-a: co się zmienia, dlaczego i jak zostało sprawdzone.

---

## 23. Agenci, którzy przeglądają kod

### Slajd

- Umiejętność przeglądu kodu (code review skill): lista kontrolna, standardy, typowe błędy zespołu
- Kilku niezależnych recenzentów: poprawność, bezpieczeństwo, prostota, zgodność z wymaganiami
- Każde znalezisko z konkretnym scenariuszem błędu
- Weryfikacja znalezisk, zanim trafią do człowieka
- Recenzent-agent zawęża pole, człowiek decyduje o scaleniu

### Notatki

- Fagan, IBM 1976: role i listy kontrolne, dziś w prompcie
- Podobne modele → podobne ślepe plamy
- OpenAI przeniosło przegląd prawie w całości na agentów, ale w produkcie beta; w systemach krytycznych rachunek jest inny

### Tekst

Skoro kod pisze agent, może go też przeglądać agent.

Po pierwsze, własny prompt albo umiejętność do przeglądu kodu z listą kontrolną Waszego zespołu: standardy, typowe błędy, zasady bezpieczeństwa. To dokładnie to, co Michael Fagan wprowadził w IBM w 1976 roku, czyli role i listy kontrolne, tylko zapisane w prompcie.

Po drugie, kilku niezależnych recenzentów z różnymi celami: poprawność, bezpieczeństwo, prostota, zgodność z wymaganiami.

Po trzecie, każde znalezisko z konkretnym scenariuszem: jakie dane wejściowe, jaki zły wynik. Do tego weryfikacja, zanim znalezisko trafi do człowieka, bo recenzenci-agenci też zmyślają.

Pamiętajmy jednak, że agenci oparci na podobnych modelach mają podobne ślepe plamy. Recenzent-agent zawęża to, na co patrzy człowiek. Nie zastępuje go w decyzji o scaleniu.

---

## 24. Symphony (1): specyfikacja → kod

### Slajd

- OpenAI Symphony (2026): publikują SPEC.md, „zbuduj to w swoim języku”
- Specyfikacja jest źródłem, kod jest generowany
- Najczystszy model kaskadowy (waterfall)?
- Wcześniejsze próby: Higher Order Software (Hamilton), CASE, Model-Driven Architecture
- Tu działa: specyfikację spisano po działającym systemie; to reimplementacja; wąska dziedzina
- Dla nowego produktu z prawdziwymi użytkownikami: skrajny waterfall

### Notatki

- Parnas i Clements 1986, *A Rational Design Process: How and Why to Fake It*
- Reeves 1992: kod źródłowy jest projektem
- Dwa generowania = dwa różne programy → potrzebne testy zgodności
- Tania regeneracja + pętla poprawek specyfikacji → bliżej modelu spiralnego
- Pytania: gdzie się uczymy? jak duża partia? co jest źródłem prawdy?

### Tekst

Na koniec przykład, który łączy wiele z tego, o czym mówiliśmy: Symphony od OpenAI, opublikowane wiosną 2026 roku. OpenAI publikuje przede wszystkim plik SPEC.md i mówi: daj go swojemu agentowi i zbuduj to w swoim języku.

Formalnie to najczystszy model kaskadowy: pełna specyfikacja na początku, implementacja w jednym przebiegu, odbiór na końcu. Ten pomysł wracał wiele razy: w Higher Order Software Margaret Hamilton, w narzędziach CASE, w Model-Driven Architecture. W ogólnym tworzeniu oprogramowania zawsze się rozbijał. Specyfikacja na tyle precyzyjna, żeby wygenerować z niej program, jest prawie tak trudna do napisania jak program, a użytkownicy dowiadują się, czego chcą, dopiero gdy widzą produkt.

Tutaj działa, bo specyfikację spisano po działającym systemie. Iteracje już się odbyły, a dokument jest ich zapisem. To reimplementacja w wąskiej, technicznej dziedzinie. Ten sam wzorzec zastosowany do nowego produktu to już skrajny waterfall.

---

## 25. Symphony (2): orkiestrator i cykl pracy nad zadaniem

### Slajd

- Tablica zgłoszeń jako miejsce sterowania (control plane)
- Każde aktywne zgłoszenie → osobny agent w osobnym katalogu
- Pętla uzgadniania stanu (jak w Kubernetesie), ponowienia, limity równoległości
- WORKFLOW.md: stany, limity i szablon promptu, wersjonowane z kodem

```
Todo → In Progress → Human Review → Rework → Merging → Done
```

- Dla każdego stanu: kto wchodzi, kto wychodzi, jaki dowód wykonania
- Ponowne uruchomienie: kontynuuj, nie zaczynaj od nowa

### Notatki

- Stan przekazania do człowieka kończy pracę agenta
- Zmienna `attempt` w szablonie: inna instrukcja przy ponowieniu
- `required_labels` jako bramka, bo treść zgłoszenia to niezaufane wejście
- Kanban: limit równoległości = limit pracy w toku
- Warunek wstępny według OpenAI: repozytorium z dobrze przygotowanym otoczeniem agenta (harness engineering)

### Tekst

Ciekawszy jest sam orkiestrator. Tablica zgłoszeń, na przykład Linear, staje się miejscem sterowania (control plane). Każde aktywne zgłoszenie dostaje własnego agenta we własnym katalogu. Orkiestrator co kilkadziesiąt sekund porównuje stan tablicy z działającymi agentami i wyrównuje różnice, tak jak pętla uzgadniania w Kubernetesie.

Zachowanie agentów opisuje plik WORKFLOW.md w repozytorium: stany, limity i szablon promptu wypełniany danymi zgłoszenia. Proces zespołu jest zapisany jawnie i wersjonowany razem z kodem.

Najważniejsza lekcja: w takim systemie trzeba precyzyjnie opisać cykl pracy nad zadaniem. Jakie są stany? Kto przenosi zgłoszenie dalej? Co musi być gotowe, żeby wyjść ze stanu? Jaki dowód wykonania zostawia agent? Kiedy czeka na człowieka? I co robi, gdy zostanie uruchomiony drugi raz: ma kontynuować, a nie zaczynać od nowa.

To tablica kanbanowa z limitem pracy w toku, na której pracują agenci. Według OpenAI działa to tylko w repozytorium z dobrze przygotowanym otoczeniem: szybkimi testami, linterami i instrukcjami.

---

## 26. Czego pilnować

### Slajd

- Nie mierzymy wierszy kodu ani liczby PR-ów
- Miary DORA + odsetek zmian poprawianych wkrótce po wdrożeniu (rework rate)
- Wrażenie przyspieszenia to słaby dowód
- Czytamy to, co scalamy
- Młodsi programiści potrzebują świadomej ścieżki nauki
- Odpowiedzialność zostaje przy człowieku, który zatwierdza

### Notatki

- Symphony: +500% scalonych PR-ów w niektórych zespołach to miara wydajności, nie wyniku
- METR: wrażenie +20%, pomiar −19%
- Koszt tokenów też jest miarą

### Tekst

Kilka słów o tym, czego pilnować. Nie mierzmy wierszy kodu ani liczby pull requestów, bo przy agentach można je zwiększać prawie bez kosztu. OpenAI podało, że w niektórych zespołach liczba scalonych PR-ów wzrosła o 500 procent. To miara wydajności, a nie wyniku. Miary DORA nadal mają sens, zwłaszcza odsetek zmian, które trzeba poprawiać wkrótce po wdrożeniu.

Nie ufajmy też wrażeniu przyspieszenia. Badanie METR pokazało, jak bardzo może mylić.

Czytajmy to, co scalamy. Młodsi programiści tracą zadania, na których kiedyś uczyli się systemu, więc potrzebują świadomej ścieżki nauki.

I najważniejsze: odpowiedzialność za kod na produkcji zostaje przy człowieku, który go zatwierdził.

---

## 27. Co wraca z historii

### Slajd

| Wtedy | Dziś, z agentami |
| --- | --- |
| Symulatory Apollo | Agent klika po aplikacji w izolowanym środowisku |
| Projektowanie na błąd astronauty | Zabezpieczenia na błąd agenta |
| Unix, powłoka, diff | Interfejs pracy agenta |
| Maszyny wirtualne (1967), chroot (1979) | Izolacja zadań i projektów |
| Najmniejsze uprawnienia (1975) | Uprawnienia agenta |
| Inspekcje Fagana (1976) | Recenzenci-agenci z listami kontrolnymi |
| TDD i BDD | Struktura i pamięć dla agenta |
| DORA: małe partie | Stosy małych PR-ów |
| CASE, MDA | Specyfikacja → kod |

### Notatki

- Karty perforowane: uruchomienie drogie → myślenie przed kodem
- Dziś: pisanie tanie, uwaga człowieka i zaufanie drogie
- Na końcu wrócić do tezy ze slajdu 2

### Tekst

Podsumujmy. Prawie wszystko, co dziś działa w pracy z agentami, kiedyś już wymyśliliśmy. Symulatory Apollo wracają jako agent, który przeklikuje aplikację w izolowanym środowisku. Projektowanie na błąd astronauty to zabezpieczenia na błąd agenta. Unix, powłoka i diff to interfejs, przez który agent pracuje. Maszyny wirtualne i chroot izolują zadania i projekty. Zasada najmniejszych uprawnień z 1975 roku mówi, co wolno agentowi. Inspekcje Fagana wracają jako recenzenci z listami kontrolnymi. TDD i BDD dają agentowi strukturę i pamięć. Małe partie z badań DORA to stosy małych PR-ów. A marzenie o generowaniu kodu ze specyfikacji wraca po raz kolejny.

W czasach kart perforowanych uruchomienie programu było drogie, więc starannie myślano przed napisaniem kodu. Dziś tanie jest pisanie kodu, a drogie są uwaga człowieka i zaufanie do wyniku. Dlatego inżynieria oprogramowania jest dziś ważniejsza niż kiedykolwiek.

---

## 28. Dziękuję

### Slajd

# Dziękuję!

Pytania?

[kontakt: uzupełnić]

### Notatki

- Podziękować, zaprosić do pytań
- Kontakt na slajdzie [uzupełnić]

### Tekst

Dziękuję bardzo za uwagę. Chętnie odpowiem na pytania.
