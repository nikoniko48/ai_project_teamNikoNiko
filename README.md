# Brief projektu: Predykcja jakości wina

## Temat
Predykcja jakości wina na podstawie jego cech chemicznych.

## Cel projektu
Stworzenie prostego systemu AI, który przewiduje jakość wina na podstawie parametrów chemicznych.

## Wartość użytkowa
- Dla użytkowników: możliwość szybkiej oceny jakości wina.  
- Dla producentów: optymalizacja procesu produkcji i rekomendacje dla konsumentów.  

## Dane
- Źródło: Wine Quality Dataset (UCI Machine Learning Repository)  
  [https://archive.ics.uci.edu/ml/datasets/wine+quality](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- Pliki: winequality-red.csv, winequality-white.csv  
- Zawartość: chemiczne parametry wina, ocena jakości (`quality`).

## Zakres projektu
1. ETL / przetwarzanie danych (Kedro)  
...

## Struktura danych
- X (features): chemiczne parametry wina (pH, siarczany, kwasy, alkohol, itd.)  
- y (target): `quality` (integer, 0–10)

## Założenia
- Projekt realizowany samodzielnie przez 2 miesiące  
- Dane podzielone na train/test  
- Model prosty regresyjny lub klasyfikacyjny (w zależności od wyboru: regresja przewiduje dokładną ocenę, klasyfikacja przewiduje kategorię jakości)
