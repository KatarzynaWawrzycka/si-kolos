# Zadanie

Szablon projektu został skonfigurowany na podstawie [Symfony Starter Kit](https://bitbucket.org/tchojna/docker-symfony-starter-kit/src/master/). W projekcie zostały przygotowane encje `Book`, `Author`, `Genre` oraz pliki pozwalające na zasilenie bazy danych losowymi danymi.

Przygotuj mechanizm edycji książki (encja `Book`). Wartości encji `Author` i `Genre`, w formularzu edycji encji `Book` powinny być pobierane z bazy danych, przy czym `Author` jest polem wielokrotnego wyboru, a `Genre` jednokrotnego.

## Reguły walidacji

* `title` - pole wymagane o minimalnej długości 3 znaki, a maksymalnej będącej długością pola w bazie danych,
* `totalPages` - pole wymagane, minimalna ilość stron to 20, a maksymalna 1200,
* `rating` - pole opcjonalne, liczba dziesiętna minimalna wartość to 0.0, a maksymalna 5.0,
* `isbn` - pole wymagane, będące poprawnym kodem ISBN,
* `publishedDate` - pole wymagane, data publikacji nie mniejsza niż 1950 rok,
* `authors` - lista autorów, każda książka musi mieć minimum jednego autora,
* `genre ` - gatunek, pole wymagane, 

## Informacje ogólne
* przesłana praca ma być pracą samodzielną,
* kod zadania ma być zgodny ze składnią zaprezentowaną na zajęciach (podział na klasy, walidacja danych, stosowanie warstwy serwisów, optymalizacja zapytań Doctrine),
* powinien przechodzić poprawnie statyczną analizę kodu zgodnie ze standardem Symfony (w katalogu projektu, w konsoli wystarczy wykonać polecenie `composer static-analysis`),
* proszę pamiętać o uzupełnieniu tłumaczeń,
* wszystkie klasy i metody powinny być poprawnie udokumentowane zgodnie ze standardem PHPDoc,
* w odpowiedzi proszę przesłać link do repozytorium _Git_ na adres: **tomasz.chojna@uj.edu.pl**