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
  Dlouhý stisk libovolného tlačítka aktivuje/deaktivuje kalibraci - "CAL " / "Endc"
 - tlačítko SET: přepíná mezi úhly (0–360) a zobrazuje např. "c 90"
 - tlačítko SAVE: uloží napětí (ve voltech) pro aktuální úhel → zobrazuje "SEtc"
 - tlačítko MAX: uloží napětí pro MAX úhel → zobrazuje "FuLL"

Po 5 minutách nečinnosti se kalibrace automaticky ukončí
EEPROM ukládá hodnoty jako float (napětí ve voltech)a
