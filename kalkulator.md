# Kalkulator
*Strona opisowa projektu*

Projekt polega na stworzeniu prostego kalkulatora w [języku C](https://pl.wikipedia.org/wiki/C_(j%C4%99zyk_programowania)).

## Spis treści
1. [Funkcjonalność](#funkcjonalność)
2. [Specyfikacja](#specyfikacja)
    1. [Schemat działania](#schemat-działania-programu-wygląda-następująco)
    1. [Wejście i wyjście](#Wejście-i-wyjście)
3. [Pomysły na nowe funkcje](#Pomysły-na-nowe-funkcje)

### Funkcjonalność

W obecnej wersji kalkulator potrafi wykonywać następujące działania:

| Działanie     | Znak do wprowadzenia |
|:------------: |:--------------------:|
| Dodawanie     | + |
| Odejmowanie   | - |
| Mnożenie | * |
| Dzielenie | / |
| Pierwiastek kwadratowy| \ |
| Potęga | ^ |

### Specyfikacja

#### Schemat działania programu wygląda następująco:

1. Wczytanie znaku działania
1. Sprawdzenie znaku instrukcją switch
    * Wczytanie odpowiedniej liczby argumentów
1. Obliczenie wyniku i wypisanie na ekran
1. Czekanie na wprowadzenie znaku przez użytkownika, aby ten zdążył obejrzeć wynik

#### Wejście i wyjście

Wejście do programu realizowane jest przez funkcje `wczytajJedna(double*)` i `wczytajDwie(double*, double*)`.
Implementacja:

```c
void wczytajDwie(double* a, double* b)
{
    printf("Podaj dwie liczby: ");
    scanf("%lf %lf", a, b);
    fflush(stdin);

    return;
}

void wczytajJedna(double* a)
{
    printf("Podaj liczbe: ");
    scanf("%lf", a);
    fflush(stdin);

    return;
}
```
### Pomysły na nowe funkcje

Oto kilka pomysłów do zrealizowania w projekcie:
- [ ] **Działanie w pętli** - póki co użytkownik może wykonać tylko jedno działanie przy uruchomieniu programu.
- [ ] **Funkcje wejścia pozwalające na formatowanie** - żeby nie trzeba było od nowa kodować w momencie, gdy przed wprowadzeniem przez użytkownika chcemy wypisać jakiś komunikat
- [ ] **Oddzielne działanie pierwiastka dowolnego stopnia** - nie jak w tej chwili dotępne jako potęga z ułamkiem w wykładniku

## Zapraszam do współpracy!
