В даному блоці перелічено основні властивості конфіг файлів. Не всі, а ті, що здались значущими особисто [msugenius](https://github.com/msugenius)

---

## Глобальний конфіг

###### Шлях до файлу  /var/www/yetiforce/config/Main.php
###### Вміст файлу
- 

---

## Налаштування режиму відладки

###### Шлях до фалу /var/www/yetiforce/config/Debug.php
###### Папка з логами (якщо включені)  /var/www/yetiforce/cache/logs/
###### Вміст файлу
-  Налаштування виводу логів
	-  Виводити в файл ($LOG_TO_FILE)
	-  Виводити в профіль ($LOG_TO_PROFILE)
	-  Вивід тексту помилки ($EXCEPTION_ERROR_TO_SHOW)
	-  Вивести трейс помилки ($DISPLAY_EXCEPTION_BACKTRACE)
---

## Безпекові налаштування 

###### Шлях до файлу: **/var/www/yetiforce/config/Security.php**
###### Вміст файлу
- *Налаштування HTTP*
	-  Примусове перенаправлення трафіку з HHTP на HTTPS ($forceHttpsRedirection)
	-  Примусове перенаправлення з помилково введеного адресу на головну сторінку ($forceUrlRedirection)
-  *Налаштування проксі*
	-  Активність проксі ($proxyConnection)
	-  Протокол для проксі конектів ($proxyProtocol)
	-  Хост проксі ($proxyHost)
	-  Порт проксі ($proxyPort)
	-  Proxy Auth (логін і  пароль) для проксі конектів ($proxyLogin та $proxyPassword)
-  *Налаштування CSP (Content Security Policy)*
	-  Дозволені джерела скриптів ($allowedScriptDomains) 
	-  Дозволені джерела фреймів ($allowedFrameDomains)
	-  Дозволені джерела форм ($allowedFormDomains)
	-  Дозволені джерела картинок ($allowedImageDomains)
	-  Повністю доступні домени ($generallyAllowedDomains)
-  *Налаштування вікна "Ціль візиту"*, що з'являється щоразу при відкритті сайту, якщо включене (VisitPurpose)
