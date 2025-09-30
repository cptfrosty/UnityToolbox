# Проблема с кодировкой скриптов при создании в Unity
Например, при создании скрипта в инспекторе он отображается так:

![alt text](https://github.com/cptfrosty/UnityToolbox/blob/main/Manuals/EncodingScripts/Media/Screenshot_1.png)

Для решения этой проблемы необходимо:
Для Visual Studio 2019/2022:
- Откройте Visual Studio
- Перейдите в Tools → Options → Environment → Documents
- Найдите опцию Save documents as Unicode when data cannot be saved in codepage
- Убедитесь, что стоит галочка
- Или выберите Unicode (UTF-8 with signature) - Codepage 65001 в настройках сохранения

И готово

![alt text](https://github.com/cptfrosty/UnityToolbox/blob/main/Manuals/EncodingScripts/Media/Screenshot_2.png)

Для меня подошло просто выставить "Unicode (UTF-8 with signature)"

![alt text](https://github.com/cptfrosty/UnityToolbox/blob/main/Manuals/EncodingScripts/Media/Screenshot_3.png)
