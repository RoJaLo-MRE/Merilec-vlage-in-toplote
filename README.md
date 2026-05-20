# Merilec-vlage-in-toplote
Ta projekt implementira merilno napravo za temperaturo in vlago z uporabo senzorja DHT22 in mikrokrmilnika Arduino Uno. Deluje na principu senzorja DHT22, ki meri relativno vlažnost zraka in temperaturo okolice ter digitalno pošilja izmerjene vrednosti na Arduino. Pridobljeni podatki se nato v realnem času prikazujejo na LCD zaslonu z I2C vmesnikom, ki omogoča enostavno priključitev z le štirimi žicami. Izpisane vrednosti so temperatura v stopinjah Celzija in relativna vlažnost v odstotkih. Ohišje je 3D tiskano in naprava kot taka bo tako lahko delovala na baterijskem ali USB napajanju.

# Komponente
- Arduino UNO
- Jumper žičke
- DHT22
- l2c LCD
- rdeča, rumena in zelena LED

# Slika vezave v easyEDA
<img width="707" height="528" alt="image" src="https://github.com/user-attachments/assets/40445dd5-b03b-4539-83db-462a4d26c054" />

# Posnetek delovanja
N/A

#Končne slike izdelka
N/A

#Komentar na delovanje
Merilec vlage in toplote vporablja DHT22 kot primarni merilec veličin. Izmerjene veličine zo izračunane in procesirane v arduino UNO in prikazane na LCD-ju. LED diode so vezane preko treh arduino pin-ov, ki so sprogramirani da čez njih spustijo napetost v odvistnosti od % izmerjene vlage.

# Prednosti
- Prenosno 3D sprintano ohišje
- Enostavna uporaba
- Enostaven napajalni sistem z 9V baterijo

# Slabosti
- Ni možna pametna uporaba preko drugih naprav
- Naprava ni modularna, za enostavno popravljanje

# Ocena natančnosti delovanja
N/A

# Analiza
N/A

# Vpliv okolja
N/A

# Zaključek
N/A

# Možne izboljšave
- Pametna uporaba naprave preko drugih naprav (mobilni telefon, PC, itd...)
- Napajanje preko USB-c priključka
