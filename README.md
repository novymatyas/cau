# **Weather Station – Raspberry Pi Pico W**



Tento projekt je určen pro Raspberry Pi Pico W a jeho úkolem je zobrazovat aktuální počasí na LCD displeji. Program se po zapnutí připojí k WiFi síti a zjistí aktuální geografickou polohu zařízení pomocí veřejné IP adresy. Poté každých deset minut načítá data o počasí z OpenWeatherMap API a zobrazuje je na displeji.



###### **Hardware**



Projekt využívá Raspberry Pi Pico W, LCD displej, USB kabel a připojení k WiFi síti. Typ LCD displeje je libovolný, například 16x2 nebo 20x4.



###### **Zapojení LCD**



LCD displej je připojen k Pico W tak, aby bylo možné zobrazovat informace o počasí a času. Všechny napájecí a datové piny musí být připojeny podle vašeho konkrétního typu displeje.



###### **Instalace a spuštění**



Nejdříve je potřeba zkopírovat projekt do počítače a vytvořit konfigurační soubor, který obsahuje údaje pro připojení k WiFi a API klíč pro OpenWeatherMap. Tento konfigurační soubor není součástí repozitáře a je chráněn před veřejným sdílením, aby nedošlo k úniku citlivých údajů.



Po vložení konfiguračního souboru a nahrání programu do Raspberry Pi Pico W se zařízení po zapnutí automaticky připojí k WiFi síti a začne zobrazovat informace na LCD displeji.



###### **Funkce programu**



Program po spuštění zobrazí hlášku „Connecting to WiFi“. Po připojení krátce ukáže souřadnice zařízení a potom začne zobrazovat aktuální počasí, včetně teploty, vlhkosti a popisu počasí.



Program je navržen tak, aby se automaticky znovu připojil k WiFi v případě výpadku a ošetřuje případné chybné odpovědi z API. Data o počasí se aktualizují každých deset minut.



###### **Rozšíření – Fork úkol**



Projekt byl rozšířen o zobrazení aktuálního času synchronizovaného přes NTP. Čas je zobrazen ve formátu hodin, minut a sekund a běží současně s informacemi o počasí na displeji.



###### **Struktura projektu**



Hlavní soubor programu je main.py. Konfigurační údaje se ukládají do souboru, který není nahráván na GitHub. Součástí projektu je také README a soubor .gitignore, který chrání citlivé údaje a nepotřebné soubory.



###### **Bezpečnost**



Citlivé údaje, jako je API klíč a přístup k WiFi, nejsou veřejně dostupné. Konfigurační soubor je ignorován při nahrávání na GitHub a všechny citlivé soubory jsou chráněny.

