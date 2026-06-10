# Merilec-vlage-in-toplote
Ta projekt implementira merilno napravo za temperaturo in vlago z uporabo senzorja DHT22 in mikrokrmilnika Arduino Uno. Deluje na principu senzorja DHT22, ki meri relativno vlažnost zraka in temperaturo okolice ter digitalno pošilja izmerjene vrednosti na Arduino. Pridobljeni podatki se nato v realnem času prikazujejo na LCD zaslonu z I2C vmesnikom, ki omogoča enostavno priključitev z le štirimi žicami. Izpisane vrednosti so temperatura v stopinjah Celzija in relativna vlažnost v odstotkih. Ohišje je 3D tiskano in naprava kot taka bo tako lahko delovala na baterijskem ali USB napajanju.

# Komponente
- 1x Arduino UNO
- žičke
- skrčki
- 1x DHT22
- 1x l2c LCD
- 1x rdeča, rumena in zelena LED
- 3x 390n upor
# Vezalna shema
<img width="707" height="528" alt="image" src="https://github.com/user-attachments/assets/40445dd5-b03b-4539-83db-462a4d26c054" />

# Shema Ohisja
<img width="711" height="459" alt="image" src="https://github.com/user-attachments/assets/8ea97ca5-6ad2-40f0-952d-aad07ab06ab8" />
<img width="658" height="462" alt="image" src="https://github.com/user-attachments/assets/c23d79c1-8df6-4628-be71-2b393e8e033f" />

# Posnetek delovanja
[MicrosoftTeams-video.mp4](https://github.com/user-attachments/assets/ac27e850-0cbb-4920-885f-2d4a0ac49804)

# Končne slike izdelka
<img width="745" height="530" alt="image" src="https://github.com/user-attachments/assets/c57a8d74-4a75-4216-ae0b-e5d934ddb0b3" />
<img width="404" height="639" alt="image" src="https://github.com/user-attachments/assets/3c273c93-67ad-4a6f-bdf8-b465a52829ac" />
<img width="499" height="632" alt="image" src="https://github.com/user-attachments/assets/f20b4c5a-6d1d-4a66-81f1-fcebc171b129" />


# Komentar na delovanje
Merilec vlage in toplote vporablja DHT22 kot primarni merilec veličin. Izmerjene veličine zo izračunane in procesirane v arduino UNO in prikazane na LCD-ju. LED diode so vezane preko treh arduino pin-ov, ki so sprogramirani da čez njih spustijo napetost v odvistnosti od % izmerjene vlage.

# Prednosti
- Prenosno 3D sprintano ohišje
- Enostavna uporaba
- Enostaven napajalni sistem z 9V baterijo

# Slabosti
- Ni možna pametna uporaba preko drugih naprav
- Naprava ni modularna, za enostavno popravljanje

# Ocena natančnosti delovanja
<img width="429" height="570" alt="image" src="https://github.com/user-attachments/assets/7db94f96-e5e3-4161-a7d0-84b686e64345" />


# Analiza
Naprava ima zelo široko merilno območje, ki sega od -10°C do 80°C. Pri katerih se meja napake tudi povečuje sorazmirno pri pre nizkih in pre visokih temperaturah. S tem lahko vidimo omejitve DHT22 senzorja.

# Zaključek

# Možne izboljšave
- Pametna uporaba naprave preko drugih naprav (mobilni telefon, PC, itd...)
- Napajanje preko USB-c priključka
