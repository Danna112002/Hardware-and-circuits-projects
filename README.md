# Hardware and Circuits Projects

Repozytorium zawiera zbiór moich projektów z zakresu elektroniki analogowej, projektowania obwodów drukowanych (PCB) oraz symulacji układów. Projekty obejmują analizę teoretyczną, symulacje SPICE, tworzenie własnych bibliotek komponentów oraz przygotowanie plików produkcyjnych płytek.

## 🛠 Wykorzystywane narzędzia
* **LTspice** – symulacje obwodów analogowych, wzmacniaczy i układów zasilania.
* **Altium Designer** – projektowanie schematów, bibliotek elementów (SchLib/PcbLib) i obwodów drukowanych (PCB).
* **LaTeX** – tworzenie dokumentacji technicznej, specyfikacji i sprawozdań z laboratoriów.

## 📁 Struktura repozytorium

### 1. D-Class Amplifier: PDM vs PWM Input Modulation
Projekt wzmacniacza audio klasy D. Głównym celem projektu jest porównanie dwóch metod modulacji sygnału wejściowego: z wykorzystaniem klasycznego komparatora (PWM) oraz modulatora Sigma-Delta (PDM).
* **Symulacje:** Modele w LTspice dla obu wariantów układu (wraz z analizą widmową FFT).
* **Dokumentacja:** Kompletne specyfikacje (wstępna, algorytmiczna i końcowa) napisane w LaTeX, zawierające schematy blokowe i przebiegi sygnałów.

### 2. Simple Amplifier Design
Kompleksowy projekt prostego wzmacniacza (w ramach przedmiotu PSEL), przeprowadzony od symulacji aż po wygenerowanie plików produkcyjnych PCB. 
* **Symulacje (LTspice):** Analiza częstotliwościowa oraz symulacja układu ze stabilizatorem napięcia, poparte sprawozdaniem.
* **Projekt PCB (Altium Designer):** 
  * Schematy ideowe (`.SchDoc`) i projekt obwodu drukowanego (`.PcbDoc`) oparte o uczelniane szablony PW.
  * Komplet plików produkcyjnych (BOM, Gerber / GerberX2, NC Drill, Pick & Place).
  * **Biblioteki:** Zestaw własnych bibliotek zintegrowanych, zawierających footprinty i symbole dla gniazd, elementów SMD (kondensatory, rezystory), regulatorów i wzmacniaczy.

### 3. Simple DC-to-DC Power Supply Chain
Projekt wielostopniowego łańcucha przetwornic napięcia stałego (DC-DC) zasilanego z 9V.
* **Symulacje (LTspice):** Poszczególne stopnie konwersji napięcia (9V na 5V, 9V na 4V, 9V na 13V, 9V na -13V) oraz ostateczna symulacja zintegrowanego, całego układu.
* **Dokumentacja:** Opis układu i wyników symulacji w pliku `Documentation_pl.pdf`.
