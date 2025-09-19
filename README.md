# C-19-09-2025
Arkusz INF.04 : 2024 - styczeń - zad. 01 

https://egzamin-programista.pl/arkusz-praktyczny-inf04-2024-01-01

Zrealizuj na podstawie tych obrazów aplikacje 
*Okno ma tło koloru CadetBlue (#5F9EA0)*
*Pola edycyjne i przycisk mają tło koloru Azure (#F0FFFF)*
*Dwa obrazy: 000-zdjecie.jpg oraz 000-odcisk.jpg. Obrazy mają tę samą wysokość. W aplikacji, której okno przedstawiono na obrazie 1 zastosowano wysokość równą 180*

<img width="903" height="396" alt="image" src="https://github.com/user-attachments/assets/294bcb89-ed1a-4805-92e2-eb4271ac2867" />

<img width="502" height="364" alt="image" src="https://github.com/user-attachments/assets/ff21bbf5-44ca-46b3-94c8-351c80a1d2fd" />

<img width="801" height="339" alt="image" src="https://github.com/user-attachments/assets/6510cf2f-d28b-49e9-aead-0ed5057c5318" />

<img width="868" height="519" alt="image" src="https://github.com/user-attachments/assets/fe6d3698-dba3-43b2-ad56-306cb2078d56" />

*Po wciśnięciu button program się wykonuje*

```
 private void button2_Click(object sender, EventArgs e)
 {

     string firstName = textBox1.Text.Trim();
     string lastName = textBox2.Text.Trim();

     // Walidacja pól
     if (string.IsNullOrEmpty(firstName) || string.IsNullOrEmpty(lastName))
     {
         MessageBox.Show("Wprowadź dane",
             "Błąd",
             MessageBoxButtons.OK,
             MessageBoxIcon.Warning);
         return;
     }

     // Ustalenie koloru oczu
     string eyeColor = radioButton1.Checked ? "niebieskie"
                     : radioButton2.Checked ? "zielone"
                     : "piwne";

     // Wyświetlenie komunikatu końcowego
     MessageBox.Show(
         $"{firstName} {lastName} kolor oczu {eyeColor}",
         "Podsumowanie",
         MessageBoxButtons.OK,
         MessageBoxIcon.Information
     );

```
*Za pomocą narzędzi do tworzenia aplikacji konsolowych zaimplementuj program sprawdzający poprawność numeru PESEL. Program powinien sprawdzać płeć i sumę kontrolną według opisu:*



<img width="884" height="486" alt="image" src="https://github.com/user-attachments/assets/870c47a5-938f-4a07-a6bb-988b69231a9a" />


*Założenia aplikacji:*

*Zastosowany obiektowy język programowania zgodny z zainstalowanym na stanowisku egzaminacyjnym: C++ lub C#, lub Java, lub Python*

*Numer PESEL może być przechowywany jako zmienna tekstowa albo tablica 11 liczb całkowitych lub znaków*

*Zmienna ta jest zainicjowana numerem PESEL zdającego lub w przypadku jego braku numerem 55030101193*

*Sprawdzanie płci należy zaimplementować w osobnej funkcji zwracającej typ znakowy o wartości 'K' dla kobiety oraz 'M' dla mężczyzny*

*Sprawdzanie sumy kontrolnej należy zaimplementować w osobnej funkcji zwracającej wartość logiczną true w przypadku zgodności sumy lub false w przeciwnym przypadku*

*Parametrem wejściowym obu funkcji jest zmienna przechowująca numer PESEL*

*Program główny testuje działanie funkcji i zawiera następujące operacje wejścia – wyjścia*

*Wczytanie z klawiatury numeru PESEL*

*Wypisanie płci (ustalonej przez funkcję) w postaci napisu: „Kobieta” lub „Mężczyzna” w oparciu o wczytany numer PESEL*
*Wypisanie informacji o zgodności lub niezgodności sumy kontrolnej w oparciu o wczytany numer PESEL*
*Program powinien podejmować zrozumiałą komunikację z użytkownikiem*
*W programie może być zastosowane angielskie lub polskie nazewnictwo zmiennych i funkcji*
*Program powinien być zapisany czytelnie, z zachowaniem zasad czystego formatowania kodu, należy stosować nazwy zmiennych znaczące oraz zgodne z przedstawionym algorytmem*
*Do kodu należy dołączyć dokumentację, która została opisana w części III zadania egzaminacyjnego*
*Kod aplikacji przygotuj do nagrania na płytę. W folderze konsola zapisz archiwum całego projektu o nazwie konsola.zip, plik z kodem źródłowym programu oraz plik uruchomieniowy, jeżeli istnieje.*


