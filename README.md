

# 🌦️ Stacje pogodowe – aplikacja WPF

## 📌 Opis projektu

Projekt przedstawia aplikację desktopową **Stacje pogodowe**, napisaną w języku **C#** z wykorzystaniem technologii **WPF (Windows Presentation Foundation)** w środowisku Visual Studio 2022.

Aplikacja umożliwia zarządzanie pomiarami pogodowymi pochodzącymi z różnych stacji meteorologicznych. Dane są odczytywane z pliku tekstowego, wyświetlane w tabeli oraz zapisywane do osobnego pliku.

## 🛠️ Technologie

- C#
- .NET 8
- WPF
- XAML
- Visual Studio 2022
- Git / GitHub

## ⚙️ Funkcjonalności

Aplikacja realizuje następujące funkcje:

1. **Odczyt pomiarów z pliku** – wczytywanie danych pogodowych z pliku `data.txt`.
2. **Nietypowy separator danych** – wykorzystanie średnika (`;`) do oddzielania poszczególnych wartości.
3. **Plik danych w repozytorium** – przykładowe pomiary znajdują się w pliku `data.txt`.
4. **Wczytywanie i zapisywanie danych** – możliwość wczytania pomiarów oraz zapisania ich do osobnego pliku `pomiary_zapisane.txt`.
5. **Dodawanie pomiarów** – użytkownik może dodać nowy pomiar poprzez formularz w aplikacji.
6. **Wyszukiwanie temperatur MAX i MIN** – aplikacja wyszukuje najwyższą i najniższą temperaturę oraz podświetla odpowiednie wiersze:
   - 🟢 Zielony – temperatura maksymalna.
   - 🔴 Czerwony – temperatura minimalna.
7. **Filtrowanie według stacji** – możliwość wyboru stacji pogodowej z listy rozwijanej i wyświetlenia tylko jej pomiarów.

## 📂 Struktura projektu

```text
StacjePogodoweWPF/
│
├── App.xaml
├── App.xaml.cs
│
├── MainWindow.xaml
├── MainWindow.xaml.cs
│
├── Pomiar.cs
│
├── data.txt
│
└── StacjePogodoweWPF.csproj
```

## 📄 Format pliku danych

Dane przechowywane są w pliku `data.txt`.

Każdy rekord zawiera:
- ID stacji pogodowej,
- datę pomiaru,
- temperaturę w stopniach Celsjusza,
- wartość wiatru.

Przykładowe dane:

```text
STA1; 2026-03-01; 18.5; 12.5;
STA2; 2026-03-02; 9.5; 8.0;
STA1; 2026-03-03; -3.5; 15.0;
STA3; 2026-03-04; 22.5; 5.5;
```

## 🚀 Uruchomienie projektu

1. Pobierz repozytorium z GitHub.
2. Otwórz projekt `StacjePogodoweWPF.csproj` w Visual Studio 2022.
3. Upewnij się, że masz zainstalowany .NET 8 SDK oraz obsługę aplikacji WPF.
4. Poczekaj na przywrócenie zależności.
5. Uruchom aplikację przyciskiem **Start** lub klawiszem `F5`.

## 💾 Zapis danych

Aplikacja korzysta z dwóch plików:

- `data.txt` – plik źródłowy zawierający przykładowe pomiary.
- `pomiary_zapisane.txt` – plik, do którego zapisywane są aktualne pomiary po wybraniu opcji „Zapisz pomiary”.

## 🎯 Cel projektu

Celem projektu jest praktyczne wykorzystanie języka C# i technologii WPF do stworzenia aplikacji desktopowej obsługującej pliki tekstowe, kolekcje danych, filtrowanie rekordów oraz analizę pomiarów pogodowych.

---

