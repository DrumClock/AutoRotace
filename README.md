

###############  VERZE - 1.6.2025  #####################

 - Ovládání motoru rotátoru pomocí H-můstku 
 - Snímání azimutu pomocí potenciometru (napěťový dělič)
 - Zobrazení azimutu / úhlu na displeji TM1637
 - zobrazení arimutu pomocí LED na krukové mapě
 - AUTOROTACE pomocí nastavení encoderem


 Po zapnutí (resetu) dojde k testu všech LED a Displeje
 Po tomto testu se rozsvítí modráLED na pozisi 0 (sever),
 nyní můžeme stisknout encoder a rotátor se nastaví na pozici "sever".
 Pokud tak neučiníme LED po 3s zhasne.

 Pro nastavení AUTOROTACE otočíme encoderem na požadovaný "azimut"
 a stiskneme encoder. Tím dojde k otáčení antény.
 Přerušení rotace je možné stiskem tlačítka pro manuální rotaci.

 Manuální rotace je možná pomocí tlačítek, která jsou blokována proti
 současnému tisku a rychlému změně směru. Takže mezi změnou směru je
 prodleva 1s, toto zabrání k rázům a zmenší namáhání převodů rotátoru.

 Přidáno PWM řízení H-můstku BTS7960, možno definovat čas
 'rampTimeUp' a 'rampTimeDown' pro plynulý rozjezd a dojezd.


 Kalibrace potenciometru pomocí tlačítek SET,SAVE,MAX
 Uložení / Načtení z EEPROM při restartu

 Funkce:
  Krátkým stiskem načteme 3 uložené předvolby kalibrace pro různé rotátory
   Tlačítko SET  - pro rot1 
   Tlačítko SAVE - pro rot2
   Tlačítko MAX  - pro rot3

  Dlouhý stisk libovolného tlačítka aktivuje/deaktivuje kalibraci - "CAL+číslo rotatoru" / "Endc" (při deaktivaci dojde k restartu MCU) 
   Tlačítko SET  - přepíná mezi kalibračnímy úhly (0–360) a zobrazuje např. "c 90"
   Tlačítko SAVE - uloží napětí (ve voltech) pro aktuální úhel → zobrazí "SEtc" a nastaví další úhel např. "c180"
   Tlačítko MAX  - uloží napětí pro MAX úhel → zobrazuje "FuLL" ukončí kalibraci a restartuje MCU

 Po 5 minutách nečinnosti se kalibrace automaticky ukončí (bez restartu MCU)



video:  https://youtu.be/hEBSZyiuYrg

 
