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

1. **ETL / przetwarzanie danych (Kedro)**  
   Wczytanie danych z CSV, czyszczenie braków i wstępna analiza.
2. **Przygotowanie danych (preprocessing)**  
   Normalizacja cech i podział na zbiory treningowe i testowe.
3. **Trening modelu ML**  
   Prosty model RandomForest lub XGBoost do przewidywania jakości wina.
4. **API backend (FastAPI)**  
   Endpoint `/predict` do wysyłania parametrów wina i odbierania przewidywanej jakości.
5. **UI frontend (Streamlit)**  
   Prosty interfejs do wpisywania parametrów wina i wyświetlania predykcji.
6. **Automatyzacja (Airflow)**  
   Uruchamianie pipeline’u ETL → preprocessing → model → ewaluacja.
7. **Wdrożenie (Docker)**  
   Konteneryzacja backendu, frontendu i modelu dla łatwego uruchamiania aplikacji.

## Struktura danych
- **X (features):** chemiczne parametry wina (pH, siarczany, kwasy, alkohol itd.)  
- **y (target):** `quality` (integer, 0–10)
