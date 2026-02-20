Tento projekt je určen pro Raspberry Pi Pico W a jeho úkolem je zobrazovat aktuální počasí na LCD displeji. Program se po zapnutí připojí k WiFi síti a získá aktuální geografickou polohu zařízení pomocí veřejné IP adresy. Poté se každých 10 minut načítají data o počasí z OpenWeatherMap API a zobrazují se na displeji.



Před spuštěním je potřeba vytvořit konfigurační soubor config.json, který obsahuje název WiFi sítě, heslo a API klíč pro OpenWeatherMap. Tento soubor není součástí GitHub repozitáře a je přidán do .gitignore, aby nedošlo k úniku citlivých údajů.



Program po spuštění nejprve zobrazí hlášku „Connecting to WiFi“, následně po připojení krátce ukáže souřadnice zařízení a potom začne zobrazovat informace o počasí. Program je navržen tak, aby se automaticky znovu připojil k WiFi v případě výpadku a ošetřuje případné chybné odpovědi z API.



Projekt byl rozšířen o zobrazení aktuálního času synchronizovaného přes NTP. Čas je zobrazen ve formátu HH:MM:SS a běží současně s informacemi o počasí na displeji.



Struktura projektu je jednoduchá: hlavní soubor je main.py, konfigurace se ukládá do config.json, soubor .gitignore zajišťuje ochranu citlivých dat a README obsahuje instrukce pro instalaci a spuštění programu.



Projekt lze nahrát do Raspberry Pi Pico W pomocí MicroPythonu a prostředí Thonny. Po správném nastavení WiFi a API klíče program běží automaticky a zobrazuje počasí a čas na připojeném LCD displeji.

