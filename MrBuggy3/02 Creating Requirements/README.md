
## Tworzenie wymagań dla aplikacji
Poniższe informacje posłużyły jako podstawa testów, która pozwoliła mi stworzyć warunki testowe i w rezultacie przypadki testowe.
1. Aplikacja składa się z aplikacji klienta i aplikacji serwera.
1. Potrzebne są **trzy** wersje aplikacji klienckiej: demo, finalna i publiczna.
2. Demo zawiera tylko jedno zadanie, różniące się od zadań dostępnych w wersji ostatecznej i publicznej.
3. Wersja publiczna zostanie wydana po zakończeniu Pucharu.
4. Trzy wersje różnią się tylko ilością zadań: 1 dla wersji demonstracyjnej, 15 dla pozostałych dwóch.
5. Aplikacja musi działać
   * Windows 7/8/8.1 - aplikacja kliencka;
   * Windows 7 - aplikacja serwera.
6. Aplikacja kliencka musi dostarczać dane do aplikacji serwerowej w postaci pliku tekstowego, albo bezpośrednio przez aplikację, albo poprzez wyeksportowanie z aplikacji klienckiej, a następnie zaimportowanie przez aplikację serwerową.
7. Aplikacja kliencka musi umożliwiać użytkownikom znalezienie jednego defektu w każdym ćwiczeniu/zadaniu i zgłoszenie go.
8. Aplikacja kliencka musi wygenerować dziennik zdarzeń.
9. Wszystkie ćwiczenia/zadania muszą być zaimplementowane w aplikacji.
10. Ćwiczenia/zadania muszą zawierać wady funkcjonalne, użytkowe lub bezpieczeństwa.
11. Ćwiczenia/zadania muszą być pokazane w losowej kolejności.
11. Aplikacja kliencka musi działać w dwóch trybach:
    * drużyna: tryby kapitana i członka drużyny;
    * indywidualny: tryb gracza.
15. Zgłaszanie usterek należy zablokować w trybie członka zespołu.
13. Aplikacja nie może utracić żadnych danych w przypadku nagłej awarii.
14. Za każdym razem, gdy klikniesz „Zgłoś usterkę”, należy utworzyć kopię zapasową. Kopia zapasowa musi być w formacie tekstowym.
15. W przypadku utraty połączenia użytkownik powinien nadal mieć możliwość korzystania z aplikacji.
16. Całe GUI musi być w języku polskim.
17. Okno aplikacji powinno zostać podzielone na dwie części: „Zadania” (Ćwiczenia/Zadania) oraz „Menu boczne” (Menu boczne).
18. Menu boczne musi składać się z okienek wyświetlających:
    * czas pozostały do ​​końca rundy (wersja ostateczna),
    * nr ćwiczenia/zadania,
    * „Opis zadania” – opis ćwiczenia/zadania,
    * „Lista zadań” wykaz zadań/ćwiczeń,
    * przyciski nawigacyjne: „Następne” (Następny) i „Poprzednie” (Poprzedni),
    * przycisk „Zaraportuj defekt” (Zgłoś błąd),
    * Przycisk "Zakończ" (Zakończ).
19. Okno ćwiczenia/zadania musi pokazywać aktualnie wykonywane ćwiczenie/zadanie.
20. Okno aplikacji musi zawierać ikonę MrBuggy 3.
21. „Opis zadania” powinny również zawierać liczbę możliwych do zdobycia punktów.
22. „Lista zadań” ma umożliwiać nawigację między zadaniami/zadaniami, a także jasno pokazywać aktualne zadanie, zadania bez odpowiedzi oraz te, na które udzielono odpowiedzi.
23. Przycisk "Zakończ" ma wyeksportować wszystkie odpowiedzi na serwer/plik tekstowy. Tej czynności nie można cofnąć i można ją wykonać tylko raz. Czynność tę należy potwierdzić w osobnym komunikacie.
24. Aplikacja serwera musi być dostępna z wiersza poleceń lub GUI i jest dedykowana wyłącznie jury turnieju.
25. Aplikacja serwera musi:
    * pobrać raporty wszystkich zespołów i użytkowników;
    * prowadzić tablicę wyników z podziałem na wyniki drużynowe i indywidualne;
    * automatycznie sprawdza zgłoszone usterki;
    * zezwolić jury na ręczną zmianę punktacji;
    * pokaż ogólną rangę na osobnym monitorze;
    * pozwalają na wygenerowanie raportu zbiorczego zawierającego pozycję użytkownika w rankingu, nazwę użytkownika i jego zespół, liczbę punktów przyznanych za każde zadanie/ćwiczenie wykonane przez każdego członka i zespół oraz sumę punktów zdobytych przez każdy zespół członek i cały zespół;
29. Rejestruj wszystkie zdarzenia (tj. [nie]pomyślnie odebrany raport lub poprawnie przejrzany raport) w dzienniku serwera.
30. Czas odpowiedzi interfejsu powinien być krótszy niż 1 sek.
31. Raport ogólny powinien zostać wygenerowany w czasie poniżej 15 sek.
32. Kopia zapasowa aplikacji klienckiej nie powinna przekraczać 2 MB.
33. Aplikacja kliencka nie może używać więcej niż 100 MB pamięci RAM.
33. Aplikacja serwera musi mieć możliwość odbierania 50 raportów naraz.
34. Dostęp do aplikacji serwera musi być chroniony loginem i hasłem.
35. Użytkownicy aplikacji klienckiej mogą tworzyć konta lub korzystać z aplikacji w trybie gościa.
35. Każdy użytkownik aplikacji serwerowej musi mieć osobny login, który składa się z 4-8 znaków (co najmniej jedna mała litera, jedna wielka litera, jedna cyfra 0-9 i jeden znak specjalny).
36. Login do aplikacji serwera nie może zawierać spacji i/lub polskich znaków diakrytycznych).
37. Hasło do aplikacji serwera musi zawierać co najmniej 4 znaki (co najmniej jedną małą literę, jedną dużą literę, jedną cyfrę 0-9 i jeden znak specjalny).
38. Hasło nie może zawierać spacji i/lub polskich znaków diakrytycznych).
39. Każdy użytkownik aplikacji klienckiej, który zdecyduje się na utworzenie konta, musi utworzyć nazwę użytkownika, podać swój adres e-mail i ustawić hasło.
40. Nazwa użytkownika w aplikacji klienckiej nie może przekraczać 100 znaków (dozwolone są białe znaki, polskie znaki diakrytyczne i inne znaki specjalne znajdujące się na klawiaturze).
41. Hasło w aplikacji klienckiej nie może przekraczać 15 znaków.
42. Hasło do aplikacji klienckiej musi zawierać co najmniej 6 znaków (co najmniej jedną małą literę, jedną dużą literę, jedną cyfrę 0-9).
43. Hasło może zawierać jeden z następujących znaków specjalnych: !@#$%^&*
44. Hasło nie może zawierać spacji i/lub polskich znaków diakrytycznych).
45. Musi istnieć procedura tworzenia, przywracania i odblokowywania konta.
46. ​​Konieczna jest procedura zmiany hasła.
47. Konto należy zablokować po trzech próbach wprowadzenia błędnego hasła.
48. Aplikacja serwera ma utworzyć kopię zapasową raportu ogólnego.
49. MrBuggy3 musi być przenośną aplikacją w archiwum zip. Archiwum musi zawierać plik exe oraz wszystkie niezbędne biblioteki i zasoby do jego uruchomienia.
50. Aplikacja demonstracyjna powinna zawierać jedno z dwóch możliwych zadań/ćwiczeń:
    * Kalkulator, który może tylko dzielić. Wada polega na tym, że dzieli się przez 0 i jako wynik pokazuje 0.
    * Funkcja, która sprawdza, czy przecinają się dwa prostokąty, a następnie wyświetla informacje. Wada to błędna informacja mówiąca, że ​​prostokąty nie przecinają się, gdy jeden z nich całkowicie zakrywa drugi.
51. Wady są punktowane według ich stopnia zaawansowania:
    * błahe wady (1-2 punkty);
    * normalne wady (3-4 punkty);
    * wady krytyczne (4-6 punktów).
52. Aplikacja odejmuje 2 punkty za zgłoszenie poprawnej funkcjonalności.
