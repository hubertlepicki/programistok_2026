# Źródła

Źródła faktów użytych w prezentacji. Pozycje oznaczone ⚠️ warto potwierdzić przed wystąpieniem: są podane z pamięci albo z omówień, a nie ze źródła pierwotnego.

## Historia

- **Definicja inżynierii oprogramowania (slajd 3)**: IEEE Std 610.12-1990, *IEEE Standard Glossary of Software Engineering Terminology*, hasło „software engineering”, punkt (1). To samo brzmienie w ISO/IEC/IEEE 24765 i SEBoK: <https://sebokwiki.org/wiki/Software_Engineering_(glossary)>.

- **Apollo, pamięć i oprogramowanie lotu**: David A. Mindell, *Digital Apollo: Human and Machine in Spaceflight*, MIT Press, 2008. ⚠️ Liczby pamięci (około 36 tys. słów stałej, 2 tys. roboczej) dotyczą komputera Block II.
- **Margaret Hamilton, termin „software engineering”, historia z programem P01 i Apollo 8**: wywiady i materiały MIT / Draper Laboratory. ⚠️ Anegdotę o córce i Apollo 8 Hamilton opowiada w wielu wywiadach, szczegóły różnią się w zależności od wersji.
- **Alarmy 1201 i 1202 w Apollo 11**: materiały historyczne NASA, Mindell (jak wyżej).
- **Konferencje NATO 1968 i 1969**: raporty zredagowane przez Petera Naura i Briana Randella (1968) oraz Johna Buxtona i Briana Randella (1969), dostępne na stronie Briana Randella: <http://homepages.cs.ncl.ac.uk/brian.randell/NATO/>. ⚠️ Liczba uczestników (około 50).
- **Fazy w projekcie SAGE**: Herbert D. Benington, *Production of Large Computer Programs*, 1956 (przedruk w *Annals of the History of Computing*, 1983).
- **Model kaskadowy**: Winston W. Royce, *Managing the Development of Large Software Systems*, IEEE WESCON, 1970.
- **Normy wojskowe**: MIL-STD-1679 (1978), DOD-STD-2167 (1985), DOD-STD-2167A (1988), MIL-STD-498 (1994). Przeglądy techniczne (SRR, PDR, CDR): MIL-STD-1521.
- **COCOMO**: Barry W. Boehm, *Software Engineering Economics*, 1981.
- **SEI i CMM**: Software Engineering Institute, Carnegie Mellon University (1984); CMM wersja 1.0 (1991).
- **Podział czasu i maszyny wirtualne**: CTSS (MIT, 1961); CP-67 (IBM Cambridge Scientific Center, 1967).
- **Unix i narzędzia**: Unix (1969), C (1972), potoki (1973), diff (Unix 5th Edition, 1974; J. W. Hunt, M. D. McIlroy, *An Algorithm for Differential File Comparison*, 1976), patch (Larry Wall, 1985), make (Stuart Feldman, 1976), SCCS (Marc Rochkind, 1972), lint (1978), chroot (Unix Version 7, 1979). Filozofia Uniksa: przedmowa McIlroya w *Bell System Technical Journal*, 1978.
- **Zasada najmniejszych uprawnień**: Jerome H. Saltzer, Michael D. Schroeder, *The Protection of Information in Computer Systems*, Proceedings of the IEEE, 1975.
- **No Silver Bullet**: Frederick P. Brooks Jr., *No Silver Bullet — Essence and Accident in Software Engineering*, IFIP 1986; *IEEE Computer*, 1987.
- **Inspekcje kodu**: Michael E. Fagan, *Design and Code Inspections to Reduce Errors in Program Development*, IBM Systems Journal, 1976.
- **Refaktoryzacja**: William Opdyke, praca doktorska, 1992; Martin Fowler, *Refactoring*, 1999.
- **Wzorce projektowe**: Gamma, Helm, Johnson, Vlissides, *Design Patterns*, 1994.
- **Manifest Agile**: <https://agilemanifesto.org/iso/pl/manifesto.html> (2001).
- **XP i TDD**: Kent Beck, *Extreme Programming Explained*, 1999; *Test-Driven Development: By Example*, 2002. ⚠️ Cytat „dobry programista ze świetnymi nawykami” jest powszechnie przypisywany Beckowi, nie sprawdzałem źródła pierwotnego.
- **BDD**: Dan North, *Introducing BDD*, Better Software, 2006.
- **Outside-in**: Steve Freeman, Nat Pryce, *Growing Object-Oriented Software, Guided by Tests*, 2009.
- **Ciągłe dostarczanie**: Jez Humble, David Farley, *Continuous Delivery*, 2010.
- **Kontenery**: Docker (2013), Kubernetes (2014).
- **DORA**: Nicole Forsgren, Jez Humble, Gene Kim, *Accelerate*, 2018; raporty na <https://dora.dev>.
- **Rodowód stacked diffs**: Phabricator (Facebook). Opcja `git rebase --update-refs`: Git 2.38 (2022).
- **git worktree**: Git 2.5 (2015).

- **Cytat Hamilton na slajdzie**: pisemny wywiad z Margaret Hamilton w: Lawrence Snyder, Ray Henry, *Fluency with Information Technology*, 7. wyd., Pearson, 2017. Transkrypcja: <https://catskull.net/interview-with-margaret-h-hamilton.html>. Inna, pierwotna wypowiedź: MIT News, *Recalling the “Giant Leap”*, 17 lipca 2009, <https://news.mit.edu/2009/apollo-vign-0717>.
- **Cytat Royce'a**: „I believe in this concept, but the implementation described above is risky and invites failure.” (Royce 1970, jak wyżej). Royce nie używa słowa „waterfall”.
- **Daty na osiach czasu**: CP-67 poprzedzał CP-40 (1964–67). lint: 1978 (publicznie w Unix V7, 1979). CruiseControl (2001) to pierwszy popularny serwer CI open source, nie pierwszy w ogóle (Tinderbox, Netscape, 1997). SUnit: artykuł Becka w *The Smalltalk Report*, 1994. JUnit: 1997.

## Agenci

- **Vibe coding**: Andrej Karpathy, post na X z 2 lutego 2025 roku.
- **Badanie METR**: *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity*, lipiec 2025: 16 programistów, 246 zadań, 19% dłuższy czas pracy z AI przy subiektywnym wrażeniu przyspieszenia o około 20%.
- **DORA a AI**: raport DORA 2024 (większe użycie AI i nieco mniejsza stabilność dostarczania) i raport DORA 2025 (AI wzmacnia istniejące praktyki). ⚠️ Warto potwierdzić dokładne sformułowania w raportach.
- **Wykorzystanie długiego kontekstu**: Nelson F. Liu i in., *Lost in the Middle: How Language Models Use Long Contexts*, 2023, arXiv:2307.03172.
- **Harness engineering**: OpenAI, *Harness engineering: leveraging Codex in an agent-first world*, luty 2026, <https://openai.com/index/harness-engineering/>.
- **Symphony**: repozytorium publiczne od marca 2026, wpis OpenAI 27 kwietnia 2026. Klucze `WORKFLOW.md` na slajdzie (`tracker.kind`, `tracker.active_states`, `agent.max_concurrent_agents`) i szablon Liquid pochodzą z SPEC.md. <https://github.com/openai/symphony>, specyfikacja: <https://github.com/openai/symphony/blob/main/SPEC.md>.
- **Symphony w prasie**: InfoQ, *OpenAI Open-Sources Symphony, a SPEC.md for Autonomous Coding Agent Orchestration*, maj 2026, <https://www.infoq.com/news/2026/05/openai-symphony-agents/>. ⚠️ Liczba „+500% scalonych PR-ów” pochodzi z omówień wpisu OpenAI. Sam wpis nie był dla mnie dostępny.
- **Specyfikacja a model kaskadowy**: David L. Parnas, Paul C. Clements, *A Rational Design Process: How and Why to Fake It*, IEEE TSE, 1986; Jack W. Reeves, *What Is Software Design?*, C++ Journal, 1992.
