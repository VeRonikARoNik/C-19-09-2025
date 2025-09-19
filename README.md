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



