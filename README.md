# Projekt AI: Predykcja jakości wina

## Temat
Predykcja jakości wina na podstawie jego cech chemicznych.

## Cel projektu
Celem projektu jest stworzenie kompletnego pipeline’u ML, który przewiduje jakość wina (ocenę 0–10) na podstawie parametrów chemicznych. Pipeline obejmuje ETL, modelowanie, API i prosty frontend do testowania predykcji.

## Wartość użytkowa
- Dla użytkowników: szybka ocena jakości wina na podstawie parametrów chemicznych.  
- Dla producentów: optymalizacja produkcji i rekomendacje dla konsumentów.

## Dane
- Źródło: Wine Quality Dataset (UCI Machine Learning Repository)  
  [https://archive.ics.uci.edu/ml/datasets/wine+quality](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- Pliki: `winequality-red.csv`, `winequality-white.csv`  
- Zawartość: chemiczne parametry wina (pH, siarczany, kwasy, alkohol itd.) oraz ocena jakości (`quality`).

## Zakres projektu (wstępny)
1. **ETL / przetwarzanie danych** (Kedro)  
   - Wczytanie danych z CSV, czyszczenie braków, wstępna analiza  
2. **Przygotowanie danych (preprocessing)**  
   - Normalizacja / standaryzacja cech, podział na zbiory train/test  

## Struktura danych
- **X (features):** chemiczne parametry wina (pH, siarczany, kwasy, alkohol itd.)  
- **y (target):** `quality` (integer, 0–10)
