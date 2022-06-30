
## Analiza specyfikacji

Przede wszystkim przeanalizowałem wymagania zawarte w [oficjalnym pliku pdf](http://mrbuggy.pl/mrbuggy3/dfiles/Specyfikacja_Mr_Buggy_3.pdf).

Poniżej znajdują się problemy, nieścisłości lub błędy, które znalazłem.

Id| Strona nr | Błąd/niepewność | Mój komentarz
--|--|--|--
1|6|Wymagane są **cztery** wersje aplikacji aplikacji|Wymienione są tylko trzy, a trzy są wymienione wcześniej w tekście
2|7|Wersja demonstracyjna,końcowa i publicznaznana tylko się tylko szczyty. Pozostałe cechy aplikacji są takie same.|Niewystarczająco konkretne. Czy to oznacza, że ​​wersja publiczna musi zawierać wybór między trybem drużynowym a trybem pojedynczym? Czy inna liczba zadań odnosi się do aplikacji demonstracyjnej w porównaniu do pozostałych dwóch, czy też wersja publiczna ma również inną liczbę zadań niż wersja ostateczna?
3|7|W śródlądowych zadaniach obsługi nie może być zadanie z wykonania demonstracyjnego (**opisane poniżej**).|Zadanie nie zostało opisane bezpośrednio poniżej. Można go znaleźć na s. 13-14.
4| 7, 8, 10|Wersja demonstracyjna, końcowa oraz publicznaznana się różnią się jedynie jedynymi.|Jest to niezgodne z późniejszymi informacjami na s. 8, który mówi, że członek zespołu NIE MOŻE zgłaszać usterek; następnie na str. 10 mówi się, że funkcja jest dostępna we wszystkich trybach.
5|7|Język programowania oraz baza danych **urzyta** podczas etapu tworzenia aplikacji nie są gotowe literówka
6|7|plikacja MrBuggy 3 się z dwóch części|części składanej składaa, część serwerowa więc w definicjach nie są to nazywane „częściami”, ale „aplikacjami”.
7|8|W każdym **zdaniu** jest nawierzchnia jednego defektu. Defekty te mogą naleźć do grup: defektów funkcjonalnych, bezpieczeństwa, użyteczności|a typo
8|8/9|pia zapasowa ma być każdorazowo po każdorazowym konie w „Znalazłem defekt”.|Gdzie indziej w dokumencie przycisk jest nazwany „Zgłoś błąd” po polsku w sposób neutralny pod względem płci, a tutaj pokazuje płeć męską .
9|10|Polak „Czas” - wyświetla czas do zakończenia rundy|Czy dotyczy to również publicznej wersji aplikacji, czy tylko finałowej wersji turniejowej?
10|10|Polak „Czas” - wyświetla czas do zakończenia godzindy (format: gg:mm:ss; minuta, minuta, sekunda, **milisekunda**)| Format nie obejmuje milisekund.
11|10|Polak „Zadania” – podaje numer N, w oknie „Zadania”. Zasady numeracji elektryczności są dostarczane.|Poniżej nie są one opisane.
12|10|Przyciski przyszłe - „Następne” i „Poprzednie” umożliwiły postępy w przyszłym**, przyszłego zadania.|Nie można nawigować do bieżącego zadania, należy porzucić.
13|10|Zakończę” - Praca nad zadaniami i odpowiedzią na ocenę. Nie da się cofnąć tej czynności. można ją zrobić tylko raz. Aby warsztaty użytkownicy musieli potwierdzać wykonanie tej czynności. Nie wiadomo, czy w potwierdzeniu zakończenia zadania pojawia się jeszcze jedno wystąpienie słowa „Zakończ”. Należy określić, jak powinno wyglądać okno potwierdzenia.
14|10|Nie da się cofnąć tej czynności **. m**ożna ją punkt|Błąd interpunkcyjny.
15|10, 11|Po wczytaniu „Zakończenia” wszystkie dane dotyczące użytkownika oraz rozwiązane przez tajne dokumenty testowe eksportowane są do pliku **binarnego**.|Rozdział 5 stwierdza, że ​​wyeksportowany plik powinien być plikiem tekstowym, a nie binarnym.
16|11|Okno powinno się mieścić w całości na aplikacji aplikacji 768 o rozdzielczości 1024x i być **estetyczne**.|"Gustowne" nie jest opisem faktycznym i powinno być dalej zdefiniowane.
17|11|W oknie aplikacji musi się znaleźć ikona MrBuggy 3.|Wymaga doprecyzowania, co oznacza „ikona”.
18|11|Zdjęcie 1|Poprzedni opis nie zawiera statusu połączenia.
19|11|Ilustracja 1|Projekt zawiera 12 widocznych zadań, podczas gdy rozdział 5.1 stwierdza, że ​​powinno ich być 15.
20|11|Aplikacja aplikacja ma zostać stworzona przy końcu języka Java7.| Na str. 7 stwierdzono, że nie należy definiować języka programowania.
21||czas odpowiedzi na koniec musi być 12 od 1 sekundy|może być problem: czas oczekiwania użytkownika może być zbyt długi dla użytkownika
22|12|kopułka z kopią aplikacji z zapasową aplikacją **2MB1**|Jaki jest ostateczny rozmiar aplikacji?
23|12|wydajność aplikacji liczona ze wzoru:|wzór nie oblicza skuteczności aplikacji.
24|12|dostęp do części serwerowej aplikacji musi być zabezpieczony loginem i mam (i kolejne punkty)|A co z aplikacją kliencką? Czy to dotyczy również tego?
25|12|w muzyce składa się z 2 do 8 dysków i używaj jednej wspólnej litery, jedną wielką literę, jedną cyfrę i jeden specjalny specjalny|Wymagania dotyczące logowania są sprzeczne – minimalna długość znaku powinna wynosić 4.
26|12|in nie może zawierać białych słów napisów: angielskich ani polskich znaków **diakrytycznych**|niewłaściwych znaków diakrytycznych.
27|12|ma musi składać się z co 20 instrukcji obsługi|długość hasła wydaje się niepotrzebnie długa.
28|13|sło nie może zawierać białychhatycznych znaków ani polskich znaków **dialekki**|niewłaściwe słowo: znaki diakrytyczne (znaki diakrytyczne).
29|13|ma być mające miejsce w zaszyfrowanym formacie.
30|13|konto musi zostać zablokowane po 3 krotnym wczytaniu **błędnego hasła lub jego części**|niepotrzebne "ze swojej części"
31|13|tokeny do konta mają być losowo|Rodzaj tokenów nie jest zdefiniowany.
32|13| Wydaje się, że może być nowa aplikacja, jedna kolejka, jeśli chcesz, jeśli uznasz, że aplikacja będzie działać tylko w trakcie przeglądu - aktualizacja .
33|13|przełączanie pomiędzymi nie może być zadaniami zadania niż 1 sekunda|czas przejścia wydaje się być zbyt długi.
34|13|Nie jest instalatorem aplikacji.|Wykaz definicji na s. 5 zawiera termin „instalator” oraz fakt, że zainstaluje aplikację.
35|14|Opis zadań|Opisanych w tej wersji|Lista zawiera dwa zadania, natomiast w rozdziale 3 podano jedno.
36|14|defekty normalne (od 3 do **4** pkt), defekty krytyczne (od **4** do 6 pkt)|Czy kryteria punktacji celowo się pokrywają?
37|wszystkie strony|często brakuje znaków interpunkcyjnych na listach|Styl powinien być spójny i tworzony zgodnie z ogólnie przyjętymi zasadami.
