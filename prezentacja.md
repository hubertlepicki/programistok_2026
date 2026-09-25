---
tytul: Inżynieria oprogramowania w dobie agentów AI
wydarzenie: Programistok 2026
prelegent: Hubert Łępicki
czas_minut: 30
---

# Inżynieria oprogramowania w dobie agentów AI

---

## Powitanie

Dzień dobry! Bardzo się cieszę, że mogę być z Wami na Programistoku. Dziękuję organizatorom za zaproszenie, a Wam za to, że wybraliście tę salę.

Nazywam się Hubert Łępicki. [Dwa, trzy zdania o sobie.]

Na początek krótkie pytanie. Podnieście rękę, jeśli używaliście kiedyś agenta kodującego: Claude Code, Codexa, Cursora albo Copilota w trybie agenta. [Pauza.] A teraz ręka w górze, jeśli robicie to codziennie w pracy. [Pauza.] Dziękuję. Dlatego dziś nie będę mówił o tym, który agent jest najlepszy, tylko o tym, jak z nimi pracować, żeby powstawało dobre oprogramowanie.

---

## Plan

Plan jest taki. Przez pierwsze kilkanaście minut szybko przejdziemy przez historię: od programu Apollo, przez konferencje NATO, Uniksa, programowanie obiektowe i agile, aż po DevOps i GitHuba. Prawie każda dobra praktyka pracy z agentami, którą dziś odkrywamy, ma swój odpowiednik sprzed dwudziestu, czterdziestu albo sześćdziesięciu lat.

W drugiej, dłuższej części porozmawiamy o agentach: dlaczego szybkie generowanie kodu bez dyscypliny kończy się źle, co pomaga, jak dzielić pracę między wielu agentów, jak ich zabezpieczyć i jak przeglądać to, co wyprodukują.

Moja teza: agenci nie zastępują inżynierii oprogramowania. Sprawiają, że jest potrzebna bardziej niż kiedykolwiek.

---

## Margaret Hamilton i program Apollo

Zaczynamy w latach sześćdziesiątych, od Margaret Hamilton. Kierowała w laboratorium MIT zespołem, który pisał oprogramowanie lotu dla programu Apollo.

Komputer pokładowy miał około trzydziestu sześciu tysięcy słów pamięci stałej i dwóch tysięcy słów pamięci roboczej. Program zapisywano w pamięci linowej (core rope): pracownice fabryki ręcznie przewlekały druty przez rdzenie magnetyczne. Trwało to tygodnie, więc program zamrażano na miesiące przed startem. Potem nie było już poprawek.

W połowie dekady oprogramowanie się spóźniało i nie mieściło w pamięci. MIT był tu wykonawcą na kontrakcie NASA, więc NASA przydzieliła swojego inżyniera, Billa Tindalla, do nadzoru nad pracą laboratorium. Tindall pilnował harmonogramu i budżetu pamięci, wymuszał decyzje, co wyciąć, i wprowadzał kontrolę zmian.

Właśnie wtedy Hamilton zaczęła nazywać swoją pracę inżynierią oprogramowania (software engineering). Na początku się z tego śmiano. Ona chciała, żeby oprogramowanie traktowano tak poważnie jak sprzęt, bo od niego zależało życie astronautów.

---

## Jak pracował zespół Apollo

Jak ten zespół pracował? Programu nie dało się przetestować w kosmosie, więc testowano go w symulacji. Były symulatory cyfrowe na dużych komputerach i symulatory hybrydowe, w których prawdziwy komputer pokładowy pracował w symulowanym otoczeniu. Testy miały kilka poziomów, aż po pełne próby misji z astronautami. Wydruki kodu czytano wspólnie, a zmiany przechodziły przez komisję.

Najważniejsze było jednak założenie, że błędy się zdarzą. Córka Hamilton, bawiąc się symulatorem, uruchomiła w trakcie lotu program przedstartowy i skasowała dane nawigacyjne. Hamilton usłyszała, że astronauta nigdy tego nie zrobi. W czasie misji Apollo 8 Jim Lovell zrobił dokładnie to, a zespół miał gotową procedurę naprawczą.

Podczas lądowania Apollo 11 komputer był przeciążony i zgłaszał alarmy 1201 i 1202. Dzięki priorytetom zadań i restartom bez utraty stanu utrzymał to, co najważniejsze. Do każdej z tych praktyk wrócimy przy agentach.

---

## NATO 1968: dyscyplina dostaje nazwę

Termin rozpowszechniła instytucja, której mało kto by się tu spodziewał: NATO. W 1968 roku w Garmisch i rok później w Rzymie Komitet Naukowy NATO zorganizował konferencje o inżynierii oprogramowania.

Dlaczego NATO? Po Sputniku sojusz uznał, że musi wzmacniać zachodnią naukę, i powołał Komitet Naukowy. Pod koniec lat sześćdziesiątych obrona powietrzna, wczesne ostrzeganie i dowodzenie zależały od coraz większych programów, które były spóźnione, drogie i zawodne. W przemyśle było tak samo, a symbolem stał się system OS/360 firmy IBM. Mówiono o kryzysie oprogramowania (software crisis). Do tego Europa bała się, że zostaje w tyle za Ameryką.

Nazwę wybrano celowo, jako prowokację: ta dziedzina jeszcze nie jest inżynierią, ale powinna nią być. Efekt? Po kilku latach istniały już czasopismo, konferencja ICSE i przedmioty na uczelniach. Dyscyplina dostała nazwę i program.

---

## Wojsko i administracja formalizują proces

Przez kolejne dekady największym zamawiającym oprogramowanie były wojsko i administracja. To one sformalizowały, jak się oprogramowanie zamawia, wycenia, projektuje i odbiera.

Już w 1956 roku Herbert Benington opisał fazy budowy systemu obrony powietrznej SAGE. W 1970 roku Winston Royce z firmy zbrojeniowej TRW opisał to, co później nazwano modelem kaskadowym (waterfall), choć sam ostrzegał przed czysto jednokierunkowym przebiegiem.

Umowy wymagały faz, dokumentów i formalnych przeglądów wymagań i projektu. Normy Departamentu Obrony opisywały, co ma powstać w każdej fazie. Do wyceny powstały modele kosztów, na przykład COCOMO Barry'ego Boehma. Pentagon sfinansował Software Engineering Institute, który stworzył model dojrzałości CMM do oceny dostawców.

To dało przewidywalność i jasną odpowiedzialność. Późna zmiana wymagań była jednak bardzo droga, a testy przychodziły na końcu. Wrócimy do tego przy generowaniu kodu ze specyfikacji.

---

## Lata 60. i 70.: narzędzia, których agenci używają do dziś

Teraz kilka wynalazków, z których agenci korzystają dosłownie.

Systemy z podziałem czasu (time-sharing), jak CTSS z 1961 roku, pozwoliły wielu osobom pracować na jednym komputerze jednocześnie. W 1967 roku IBM uruchomił CP-67: każdy użytkownik dostawał własną, izolowaną maszynę wirtualną.

Potem przyszły Unix i język C. Doug McIlroy wymyślił potoki (pipes) i opisał filozofię Uniksa: małe programy, które robią jedną rzecz dobrze i komunikują się tekstem. Do tego doszły powłoka i skrypty, diff do porównywania wersji, później patch do nakładania zmian, make do budowania, SCCS do kontroli wersji i lint do wyłapywania podejrzanego kodu. W 1979 roku pojawił się chroot, przodek kontenerów. A w 1975 roku Saltzer i Schroeder opisali zasadę najmniejszych uprawnień (least privilege).

Agent kodujący to w praktyce program, który pracuje w powłoce, używa grepa, gita i testów, a swoje zmiany pokazuje jako diff. Tekstowy interfejs Uniksa okazał się idealny dla modeli językowych.

---

## Lata 80. i 90.: obiekty, modele, generatory kodu

Lata osiemdziesiąte i dziewięćdziesiąte to programowanie obiektowe. Smalltalk z Xerox PARC dał obiekty i żywe środowisko programistyczne, a później pierwsze narzędzie do automatycznej refaktoryzacji i framework testów SUnit. Ze społeczności Smalltalka wyszły też wzorce, pierwsza wiki i programowanie ekstremalne.

Przyszły C++, Eiffel z projektowaniem przez kontrakt, katalog wzorców projektowych, książka Fowlera o refaktoryzacji, a w 1997 roku UML. Narzędzia CASE obiecywały, że kod będzie generowany z diagramów. Obietnice były dużo większe niż efekty.

W 1986 roku Fred Brooks napisał esej *No Silver Bullet*. Oddzielił w nim złożoność przypadkową, wynikającą z narzędzi, od złożoności istotnej, wynikającej z samego problemu. Napisał, że żadna pojedyncza technologia nie da dziesięciokrotnej poprawy. Warto to pamiętać, gdy ktoś obiecuje, że AI napisze za nas cały system.

---

## Agile: XP, TDD i BDD

W 2001 roku siedemnaście osób napisało Manifest Agile. Ważniejsze od nazwy były jednak praktyki, zwłaszcza z programowania ekstremalnego (Extreme Programming) Kenta Becka: programowanie w parach, ciągła integracja, małe wydania i ciągła refaktoryzacja.

Dla nas najważniejsze jest TDD, czyli programowanie sterowane testami (test-driven development). Najpierw piszesz mały test, który nie przechodzi: czerwony. Potem najmniej kodu, żeby przeszedł: zielony. Potem porządkujesz kod przy zielonych testach: refaktoryzacja. I od nowa. Ważny szczegół: czerwony test trzeba zobaczyć i sprawdzić, że pada z właściwego powodu. Test, który przechodzi od razu, niczego nie dowodzi.

Kilka lat później Dan North zaproponował BDD, czyli zachowanie systemu opisane przykładami: zakładając, że…, gdy…, wtedy… Takie scenariusze mogą czytać ludzie z biznesu, a uruchamiać komputer.

Kent Beck mówił o sobie, że nie jest świetnym programistą, tylko dobrym programistą ze świetnymi nawykami. Zapamiętajcie to zdanie.

---

## DevOps, infrastruktura jako kod, kontenery

Pod koniec pierwszej dekady XXI wieku powstał ruch DevOps: jeden zespół odpowiada za oprogramowanie od napisania do działania na produkcji. Pojawił się potok wdrożeniowy (deployment pipeline): każda zmiana automatycznie przechodzi przez budowanie, testy i wdrożenie.

Konfigurację serwerów zaczęto zapisywać jako kod. To infrastruktura jako kod (Infrastructure as Code): Puppet, Chef, Ansible, Terraform. Docker spakował aplikację razem ze środowiskiem, a Kubernetes zaczął zarządzać tysiącami kontenerów.

Dojrzało też podejście do sekretów. Hasła i klucze nie trafiają do repozytorium, tylko do menedżerów sekretów, które wydają je na określony czas i w określonym zakresie. Zasada najmniejszych uprawnień stała się codzienną praktyką.

Dla agentów to fundament. W minutę stawiamy powtarzalne, izolowane środowisko i dajemy agentowi dokładnie te uprawnienia, których potrzebuje.

---

## Git, pull requesty, testy, dane

Ostatni przystanek historyczny. W 2005 roku powstał Git, a w 2008 roku GitHub z pull requestami, czyli propozycjami zmian z dyskusją i przeglądem w jednym miejscu. Przegląd kodu (code review), który w latach siedemdziesiątych był formalną inspekcją w IBM, stał się codziennością. Upowszechniła się piramida testów: dużo szybkich testów jednostkowych, mniej integracyjnych, niewiele wolnych testów przez interfejs.

W 2018 roku autorzy badań DORA pokazali w książce *Accelerate*, na danych od dziesiątek tysięcy osób, że najlepsze zespoły wdrażają małe zmiany często i mają przy tym mniej awarii. Szybkość i stabilność nie są w konflikcie. Warunek to małe partie, automatyczne testy i szybka informacja zwrotna.

Tyle historii. Przejdźmy do agentów.

---

## Od podpowiedzi do agentów

W ciągu pięciu lat przeszliśmy trzy etapy. W 2021 roku narzędzia podpowiadały kolejne wiersze. Pod koniec 2022 roku zaczęliśmy z modelami rozmawiać. Od 2025 roku na dobre pracujemy z agentami.

Agent to prosta pętla: model proponuje działanie (przeczytaj plik, zmień plik, uruchom testy), program je wykonuje, a wynik wraca do modelu. I tak do skutku. Powstały też pierwsze standardy: MCP do podłączania narzędzi, AGENTS.md z instrukcjami w repozytorium i umiejętności (skills) do powtarzalnych zadań.

Wróćmy do Brooksa. Agent świetnie zmniejsza złożoność przypadkową: szablonowy kod, szukanie w dokumentacji, pamiętanie API. Nie usuwa złożoności istotnej. Nadal ktoś musi zdecydować, co system ma robić, i sprawdzić, czy to robi. Wąskie gardło przesuwa się z pisania kodu na specyfikację i weryfikację.

---

## Programowanie na wyczucie (vibe coding)

W lutym 2025 roku Andrej Karpathy nazwał nowy styl pracy: vibe coding, czyli programowanie na wyczucie. Opisujesz, czego chcesz, akceptujesz wszystko, co zaproponuje agent, i nie czytasz kodu. Do weekendowego prototypu to świetne.

Kłopot zaczyna się, gdy tak powstaje system, który ma żyć latami. Powstaje wtedy szybko dużo kodu niskiej jakości: zduplikowanego, bez testów, niespójnego, niezrozumiałego dla zespołu. Po angielsku mówi się na to slop.

To jednak nie jest nowy problem. Tak wygląda kod człowieka, który nie stosuje dobrych praktyk: nie pisze testów, nie refaktoryzuje, nie daje nikomu kodu do przeglądu. Agent robi to po prostu dziesięć razy szybciej.

W badaniu METR z 2025 roku doświadczeni programiści z narzędziami AI byli o 19 procent wolniejsi, choć byli przekonani, że pracowali o 20 procent szybciej. Raporty DORA opisują AI jako wzmacniacz: wzmacnia i dobre, i złe praktyki zespołu.

---

## Ograniczenia modeli

Skąd to się bierze? Modele mają konkretne ograniczenia.

Po pierwsze, ograniczony kontekst. Model widzi tylko część projektu i nie pamięta poprzednich sesji. Po drugie, w długiej sesji gubi wątek. Badania pokazują, że im dłuższy kontekst, tym gorzej model korzysta z informacji ze środka. Gdy kontekst się zapełnia, jest streszczany i szczegóły giną. Agent zapomina, co ustaliliście godzinę temu.

Po trzecie, luki w wymaganiach wypełnia pewnie i wiarygodnie. Nie zapyta, jeśli go do tego nie skłonimy. Potrafi też wymyślić metodę API albo pakiet, które nie istnieją. Po czwarte, gdy agent mówi „gotowe”, to jeszcze nie jest dowód, że działa.

Człowiek też ma ograniczoną pamięć roboczą i też się myli. Dlatego wymyśliliśmy praktyki, które dają zewnętrzną strukturę. Agent potrzebuje ich jeszcze bardziej.

---

## TDD jako struktura dla agenta

I tu dochodzimy do sedna. Moim zdaniem TDD to najlepsze, co możemy dać agentowi.

Po pierwsze, TDD wymusza małe kroki: jedno zachowanie, jeden test, jedna zmiana. Taki krok mieści się w kontekście modelu i łatwo go przejrzeć.

Po drugie, test napisany przed kodem jest niezależnym opisem tego, co ma się stać. Jeśli agent najpierw napisze kod, a potem test, test często utrwala błąd, bo opisuje to, co kod robi, a nie to, co powinien. Dlatego każę agentowi uruchomić nowy test i pokazać, że pada z oczekiwanym komunikatem. Dopiero wtedy wiem, że test coś sprawdza.

Po trzecie, testy są pamięcią projektu. Agent zapomni, co ustaliliśmy rano. Test nie zapomni.

Jest też pułapka. Agent, któremu każe się doprowadzić testy do zieleni, potrafi osłabić asercję albo pominąć test. Potrzebna jest twarda reguła: nie usuwamy, nie pomijamy i nie osłabiamy testów, żeby przeszły.

---

## Najpierw przykłady i pytania, potem kod

Druga rzecz: zanim agent napisze kod, ustalmy, co znaczy „gotowe”. Najlepiej przykładami, w stylu BDD. Zamiast „obsłuż wykorzystane bilety” piszemy: zakładając, że bilet został już użyty, gdy ktoś zeskanuje go przy wejściu, wtedy bramka się nie otwiera, a obsługa widzi, kiedy bilet użyto. Taki przykład od razu staje się testem akceptacyjnym. Piszemy go najpierw, patrzymy, jak pada, i schodzimy do testów jednostkowych, z zewnątrz do środka.

Agent powinien też pytać, zamiast zgadywać. Większość agentów ma tryb planowania: najpierw plan i rozmowa, potem akceptacja, a dopiero potem zmiany. Warto też zacząć od szkieletu (walking skeleton), czyli najcieńszego działającego przekroju przez cały system, zanim agent zacznie rozbudowywać szczegóły.

---

## Pętla jakości

Zielone testy to nie koniec. Po każdym cyklu przychodzi refaktoryzacja, i to nie tylko kodu, ale też testów. Agent w trakcie pracy tworzy sporo testów pomocniczych, które potem warto scalić albo usunąć.

Potem przegląd wewnętrzny. Dobrze działa drugi agent z czystym kontekstem, który nie zna uzasadnień autora i widzi tylko diff i wymagania.

Trzecie sprawdzenie: czy zmiana robi to, o co proszono, i nic więcej. Agenci lubią dodawać rzeczy przy okazji: opcje, abstrakcje na zapas, obsługę przypadków, które nie mogą wystąpić, komentarze opisujące kod.

Czwarte to standardy zespołu. Jeśli macie wytyczne (guidelines) albo księgę stylu (stylebook), zapiszcie je tak, żeby agent mógł je wczytać.

I dobra wiadomość: refaktoryzacja i usuwanie kodu nigdy nie były tak tanie. Korzystajcie z tego regularnie.

---

## Agent sam klika po aplikacji

Człowiek, zanim powie, że skończył, zwykle uruchamia aplikację i się przez nią przeklikuje. Agent może zrobić to samo. Przez Playwrighta albo Chrome DevTools, podłączone przez MCP, otwiera przeglądarkę, loguje się, przechodzi ścieżkę użytkownika, robi zrzuty ekranu, czyta konsolę, ruch sieciowy i logi serwera.

Dzięki temu wyłapuje to, czego testy jednostkowe nie widzą: rozjechany układ, zły komunikat, przycisk, który nic nie robi, przepływ, który się urywa.

To ta sama idea co w Apollo: zanim polecisz, przeleć misję w symulatorze. Zrzuty ekranu albo nagranie zostają jako dowód wykonania dla człowieka, który przegląda zmianę.

---

## Kontekst to też kod projektu

Agent zaczyna każdą sesję bez pamięci o projekcie. Wszystko, co powinien wiedzieć, musi być zapisane w repozytorium. Standardem stał się plik AGENTS.md. W lutym 2026 roku OpenAI opisało, że ich duży plik instrukcji zawiódł: nie mieścił się w kontekście, rozmywał najważniejsze reguły i szybko się starzał. Zastąpili go krótkim spisem treści, który odsyła do szczegółowych dokumentów.

Szczegóły warto pakować w umiejętności, które agent wczytuje dopiero wtedy, gdy są potrzebne.

Najważniejsza zasada: ważna reguła powinna przechodzić od formy miękkiej do twardej. Najpierw uwaga w przeglądzie, potem zdanie w dokumentacji, potem umiejętność, a na końcu linter, test albo hook, którego agent nie obejdzie. I jeszcze jedno: komunikat lintera piszcie jak instrukcję. Nie tylko co jest źle, ale też co zrobić zamiast tego.

---

## Wiele zadań naraz

Agenci pozwalają pracować nad wieloma zadaniami naraz. Najprostsze narzędzie to drzewa robocze gita (worktrees): kilka katalogów z jednego repozytorium, każdy na innej gałęzi, w każdym inny agent.

Worktree izoluje jednak tylko pliki. Jeśli aplikacja potrzebuje bazy danych i usług na konkretnych portach, agenci zaczną sobie przeszkadzać. Wtedy każde zadanie potrzebuje własnego kontenera albo maszyny wirtualnej. To ten sam pomysł, który IBM zrealizował w 1967 roku.

Dwie rzeczy są ważne. Po pierwsze, zadania muszą być naprawdę niezależne. Jeśli dwa zmieniają ten sam moduł, będą konflikty albo dwa różne rozwiązania tego samego problemu. Działa tu prawo Conwaya: podział pracy musi pasować do podziału systemu.

Po drugie, limit wyznacza człowiek. Każdy wynik trzeba przejrzeć i zintegrować. Uruchamiajcie tylu agentów, ile wyników jesteście w stanie rzetelnie ocenić.

---

## Izolacja i najmniejsze uprawnienia, ale z dostępem do wiedzy

Bezpieczeństwo. Tu ścierają się dwie potrzeby.

Pierwsza to izolacja. Każdy projekt powinien mieć osobne środowisko: własne pliki, własne sekrety, ograniczoną sieć. Agent pracujący nad jednym projektem nie powinien widzieć kluczy innego. Obowiązuje zasada najmniejszych uprawnień: żadnej produkcji, żadnych produkcyjnych danych, sekrety z menedżera, a nie z pliku. Działania trudne do cofnięcia, czyli commit, push, usuwanie i publikowanie, tylko za zgodą człowieka.

Druga potrzeba: agent bez kontekstu zgaduje. Potrzebuje dostępu do wiedzy: zgłoszeń, dokumentacji, systemu projektowego, na przykład Figmy. MCP pozwala to podłączyć, najlepiej tylko do odczytu, z wąskim zakresem i osobnym kontem dla agenta.

I jeszcze jedno: treść z zewnątrz to dane, a nie polecenia. Opis zgłoszenia czy komentarz w PR mogą zawierać tekst, który próbuje przejąć sterowanie agentem. To wstrzykiwanie poleceń (prompt injection).

---

## Pull requesty, które da się przejrzeć

Agent w godzinę może wygenerować zmianę, której przegląd zajmie człowiekowi dzień. Albo, co gorsze, zmiana zostanie przejrzana pobieżnie. Dlatego pull requesty trzeba projektować z myślą o przeglądzie.

Jedna zmiana, jeden cel. Jeśli nowa funkcja wymaga refaktoryzacji, najpierw osobny PR z refaktoryzacją bez zmiany zachowania, a potem PR ze zmianą zachowania.

Większą pracę układamy w stos zależnych PR-ów (stacked PRs): każdy buduje na poprzednim i każdy da się przejrzeć osobno. Ta praktyka wyrosła w Facebooku, a dziś wspierają ją narzędzia takie jak Graphite czy Sapling, a nawet sam git. Kiedyś największym kosztem stosu było jego utrzymanie: rebase, poprawki w środku stosu. Dla agenta to tania, mechaniczna praca.

W opisie PR-a: co się zmienia, dlaczego i jak zostało sprawdzone.

---

## Agenci, którzy przeglądają kod

Skoro kod pisze agent, może go też przeglądać agent.

Po pierwsze, własny prompt albo umiejętność do przeglądu kodu z listą kontrolną Waszego zespołu: standardy, typowe błędy, zasady bezpieczeństwa. To dokładnie to, co Michael Fagan wprowadził w IBM w 1976 roku, czyli role i listy kontrolne, tylko zapisane w prompcie.

Po drugie, kilku niezależnych recenzentów z różnymi celami: poprawność, bezpieczeństwo, prostota, zgodność z wymaganiami.

Po trzecie, każde znalezisko z konkretnym scenariuszem: jakie dane wejściowe, jaki zły wynik. Do tego weryfikacja, zanim znalezisko trafi do człowieka, bo recenzenci-agenci też zmyślają.

Pamiętajmy jednak, że agenci oparci na podobnych modelach mają podobne ślepe plamy. Recenzent-agent zawęża to, na co patrzy człowiek. Nie zastępuje go w decyzji o scaleniu.

---

## Symphony (1): specyfikacja → kod

Na koniec przykład, który łączy wiele z tego, o czym mówiliśmy: Symphony od OpenAI, opublikowane wiosną 2026 roku. OpenAI publikuje przede wszystkim plik SPEC.md i mówi: daj go swojemu agentowi i zbuduj to w swoim języku.

Formalnie to najczystszy model kaskadowy: pełna specyfikacja na początku, implementacja w jednym przebiegu, odbiór na końcu. Ten pomysł wracał wiele razy: w Higher Order Software Margaret Hamilton, w narzędziach CASE, w Model-Driven Architecture. W ogólnym tworzeniu oprogramowania zawsze się rozbijał. Specyfikacja na tyle precyzyjna, żeby wygenerować z niej program, jest prawie tak trudna do napisania jak program, a użytkownicy dowiadują się, czego chcą, dopiero gdy widzą produkt.

Tutaj działa, bo specyfikację spisano po działającym systemie. Iteracje już się odbyły, a dokument jest ich zapisem. To reimplementacja w wąskiej, technicznej dziedzinie. Ten sam wzorzec zastosowany do nowego produktu to już skrajny waterfall.

---

## Symphony (2): orkiestrator i cykl pracy nad zadaniem

Ciekawszy jest sam orkiestrator. Tablica zgłoszeń, na przykład Linear, staje się miejscem sterowania (control plane). Każde aktywne zgłoszenie dostaje własnego agenta we własnym katalogu. Orkiestrator co kilkadziesiąt sekund porównuje stan tablicy z działającymi agentami i wyrównuje różnice, tak jak pętla uzgadniania w Kubernetesie.

Zachowanie agentów opisuje plik WORKFLOW.md w repozytorium: stany, limity i szablon promptu wypełniany danymi zgłoszenia. Proces zespołu jest zapisany jawnie i wersjonowany razem z kodem.

Najważniejsza lekcja: w takim systemie trzeba precyzyjnie opisać cykl pracy nad zadaniem. Jakie są stany? Kto przenosi zgłoszenie dalej? Co musi być gotowe, żeby wyjść ze stanu? Jaki dowód wykonania zostawia agent? Kiedy czeka na człowieka? I co robi, gdy zostanie uruchomiony drugi raz: ma kontynuować, a nie zaczynać od nowa.

To tablica kanbanowa z limitem pracy w toku, na której pracują agenci. Według OpenAI działa to tylko w repozytorium z dobrze przygotowanym otoczeniem: szybkimi testami, linterami i instrukcjami.

---

## Czego pilnować

Kilka słów o tym, czego pilnować. Nie mierzmy wierszy kodu ani liczby pull requestów, bo przy agentach można je zwiększać prawie bez kosztu. OpenAI podało, że w niektórych zespołach liczba scalonych PR-ów wzrosła o 500 procent. To miara wydajności, a nie wyniku. Miary DORA nadal mają sens, zwłaszcza odsetek zmian, które trzeba poprawiać wkrótce po wdrożeniu.

Nie ufajmy też wrażeniu przyspieszenia. Badanie METR pokazało, jak bardzo może mylić.

Czytajmy to, co scalamy. Młodsi programiści tracą zadania, na których kiedyś uczyli się systemu, więc potrzebują świadomej ścieżki nauki.

I najważniejsze: odpowiedzialność za kod na produkcji zostaje przy człowieku, który go zatwierdził.

---

## Co wraca z historii

Podsumujmy. Prawie wszystko, co dziś działa w pracy z agentami, kiedyś już wymyśliliśmy. Symulatory Apollo wracają jako agent, który przeklikuje aplikację w izolowanym środowisku. Projektowanie na błąd astronauty to zabezpieczenia na błąd agenta. Unix, powłoka i diff to interfejs, przez który agent pracuje. Maszyny wirtualne i chroot izolują zadania i projekty. Zasada najmniejszych uprawnień z 1975 roku mówi, co wolno agentowi. Inspekcje Fagana wracają jako recenzenci z listami kontrolnymi. TDD i BDD dają agentowi strukturę i pamięć. Małe partie z badań DORA to stosy małych PR-ów. A marzenie o generowaniu kodu ze specyfikacji wraca po raz kolejny.

W czasach kart perforowanych uruchomienie programu było drogie, więc starannie myślano przed napisaniem kodu. Dziś tanie jest pisanie kodu, a drogie są uwaga człowieka i zaufanie do wyniku. Dlatego inżynieria oprogramowania jest dziś ważniejsza niż kiedykolwiek.

---

## Dziękuję

Dziękuję bardzo za uwagę. Chętnie odpowiem na pytania.
