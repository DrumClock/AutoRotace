# Ovládání rotátoru "SEVER"

![Rotator_frame](https://github.com/DrumClock/AutoRotace/blob/main/IMG_panel.jpg)

# Popis

 - Ovládání DC motoru rotátoru pomocí H-můstku (24V)
 - Snímání azimutu pomocí potenciometru (napěťový dělič)
 - Zobrazení azimutu na displeji TM1637
 - zobrazení arimutu pomocí LED na krukové mapě (Neopixel 60 LED)
 - nastavení AUTOROTACE encoderem KY-040
 - kalibrace snímače a uložení do EEPROM (max. 3 rotátory)

# Funkce ovládání

 Po zapnutí (resetu) dojde k testu všech LED a Displeje.
 Po testu se rozsvítí na kruhové mapě modrá LED na pozici 0 (sever),
 nyní můžeme stisknout encoder a rotátor se nastaví na pozici "sever".
 Pokud tak neučiníme LED po 3s zhasne.

 Pro nastavení AUTOROTACE otočíme **`encoderem`** na požadovaný "azimut"
 a stiskneme encoder. Tím dojde k otáčení antény.
 Přerušení rotace je možné stiskem tlačítka pro manuální rotaci.

 Manuální rotace je možná pomocí tlačítek **`CW`** a **`CCW`**, která jsou blokována proti
 současnému tisku a rychlému změně směru. Takže mezi změnou směru je
 prodleva 1s, toto zabrání k rázům a zmenší namáhání převodů rotátoru.

Kalibrace potenciometru pomocí tlačítek M1/C, M2/S, M3/F a uložení do EEPROM 


 # Funkce tlačítek "Kalibrace"

 ![Scheme_frame](https://github.com/DrumClock/AutoRotace/blob/main/IMG_kalibrace.jpg)
 
  Krátkým stiskem načteme 3 uložené předvolby kalibrace pro různé rotátory
  - Tlačítko **`M1`**  - displej zobrazí "rot1" 
  - Tlačítko **`M2`**  - displej zobrazí "rot2"
  - Tlačítko **`M3`**  - displej zobrazí "rot3"

  Dlouhý stisk libovolného tlačítka aktivuje/deaktivuje kalibraci - displej zobrazí "CAL+číslo rotatoru" nebo "Endc" (při deaktivaci dojde k restartu MCU) 
  - Tlačítko **`C`**  - přepíná mezi kalibračnímy úhly (0,90,180,270,360) a displejv zobrazuje např. "c 90"
  - Tlačítko **`S`**  - uloží napětí (ve voltech) pro aktuální úhel displej zobrazí "SEtc" a nastaví další úhel např. "c180"
  - Tlačítko **`F`**  - uloží napětí pro MAX úhel displej zobrazuje "FuLL" ukončí kalibraci a restartuje MCU

 Po 5 minutách nečinnosti se kalibrace automaticky ukončí (bez restartu MCU)


# Video:  https://youtu.be/hEBSZyiuYrg


# Schéma:
![Scheme_frame](https://github.com/DrumClock/AutoRotace/blob/main/Arduino_Sever_2.png)

# MAPA z JN69NX
- přiložený soubor **`mapa JN69NX.cdr`** je pro grafický editor **`CorelDraw`** 

![mapa_frame](https://github.com/DrumClock/AutoRotace/blob/main/mapa.png) 

 
