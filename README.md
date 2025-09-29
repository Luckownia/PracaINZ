# 📊 Generator Live Dashboard

**Generator Live Dashboard** to wszechstronny generator dashboard-ów stworzony w Streamlit, który umożliwia wizualizację danych z różnych źródeł — API, baz danych (PostgreSQL, MySQL, MongoDB) oraz strumieni kamer na żywo.

https://realtimedatadashboard.streamlit.app/
---

## 🚀 Funkcje

- 🔌 **Połączenia API** – pobieraj dane z zewnętrznych API i twórz wykresy w czasie rzeczywistym.
- 🛢️ **Obsługa baz danych** – wizualizuj dane z PostgreSQL, MySQL i MongoDB.
- 🎥 **Podgląd z kamer** – dodaj strumienie kamer i oglądaj obraz na żywo.
- 📈 **Dynamiczne wykresy** – generowanie wykresów liniowych, słupkowych i punktowych z Plotly.


---

## 🖥️ Filmy


https://github.com/user-attachments/assets/ca35fc64-9da9-4e9d-a3b0-c79e2242bab4



https://github.com/user-attachments/assets/3f9e6dac-3607-438e-b860-1f5297db30c6






https://github.com/user-attachments/assets/b4efcc29-9132-4003-83b7-33ec90d04aae






https://github.com/user-attachments/assets/7e1f2547-4e86-4cfa-8abc-3186ebd32022







https://github.com/user-attachments/assets/38bd8cfd-0c3c-4e6c-aa73-e03757c36a86









https://github.com/user-attachments/assets/ff132016-cae5-4497-938e-bfe9d661556f





https://github.com/user-attachments/assets/b85bac35-3a0c-4f8c-aaf1-9d93118bc016






https://github.com/user-attachments/assets/3d1967cd-cd53-4711-9ff1-82a1f3652997




https://github.com/user-attachments/assets/63286594-3f89-4ad6-abc2-adb010eddae0




https://github.com/user-attachments/assets/c8e63a98-1253-4edf-93be-882f3641fec3



https://github.com/user-attachments/assets/5b693d90-1e53-4654-a6be-6634c1b4501d




https://github.com/user-attachments/assets/8cc3bb87-56a1-4297-b67e-4f8123375247



---

## 🔧 Uruchamianie projektu

### 1. Klonowanie repozytorium

```bash
git clone https://github.com/Luckownia/PracaIN-.git
```

### 2. Pobranie wymaganych biblotek
```bash
pip install -r requirements.txt
```
### 3. Uruchomienie Aplikacji 

```bash
streamlit run .\main.py
```

---

## 🧪 Tryby działania aplikacji

Po uruchomieniu aplikacji w przeglądarce (domyślnie `http://localhost:8501`) w panelu bocznym możesz wybrać jeden z trybów:

### 🔹 API
- Wprowadź adres URL API oraz opcjonalne parametry zapytania w formacie JSON.
- Kliknij „Pobierz dane z API”, a następnie skonfiguruj wykres: tytuł, typ, kolumny X/Y oraz liczbę punktów.
- Obsługiwane typy wykresów: Liniowy, Słupkowy, Punktowy.

### 🔹 Baza danych
- Wybierz typ bazy: PostgreSQL, MySQL lub MongoDB.
- Wprowadź dane połączenia, zapytanie SQL lub kolekcję (dla MongoDB).
- Po załadowaniu danych wybierz kolumny do wykresu oraz jego typ.

### 🔹 Kamery
- Dodaj adres URL strumienia z kamery.
- Aplikacja pokaże obraz na żywo w czasie rzeczywistym.
- Możesz dodawać i usuwać wiele kamer dynamicznie.

---

## 🗂️ Struktura katalogów

├── main.py # Główna aplikacja Streamlit

├── charts/

│ └── plotter.py # Tworzenie wykresów (Plotly)

├── fetchers/

│ ├── api_fetcher.py # Pobieranie danych z API

│ ├── camera_fetcher.py # Obsługa kamer 

│ └── database_fetcher.py # Obsługa baz danych SQL/MongoDB/PostreSql

├── session/

│ └── state_manager.py # Utrzymywanie stanu sesji użytkownika

├── ui/

│ ├── api_config.py # UI do konfiguracji API i wykresów

│ ├── camera_config.py # UI do dodawania i zarządzania kamerami

│ └── db_config.py # UI do konfiguracji połączenia z bazą danych

└── requirements.txt # Lista biblotek
