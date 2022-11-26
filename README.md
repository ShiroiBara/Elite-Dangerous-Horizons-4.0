# Elite-Dangerous-Horizons-4.0
Руководство по запуску Горизонтов 4.0 (стим версия) для владельцев аккаунтов с купленным дополнением Odyssey

Люди, играющие в стим версию элиты и имеющие дополнение Одиссея столкнулись с проблемой невозможности поиграть с теми, у кого остались Горизонты 4.0
Имеющийся лаунчер от фронтиров не дает возможность выбрать нужную версию Горизонтов в самом лаунчере. Дело в том, что предлагаемая там версия это 3.8,
та в которой старая графика, менеее требовательные ресурсы и все те старые фишки, которые были там, начиная примерно с 2016 года. Горизонты 4.0 это графика
как в дополнении Горизонты, но без миссиё с "ногами" и высадок в режиме третье лица на станции и планеты. Побороть данную проблему можно используя следующие шаги:

1. Качаем архив https://github.com/rfvgyhn/min-ed-launcher/releases/download/v0.7.5/min-ed-launcher_v0.7.5_win10-x64.zip
2. Распаковываем его в какую-нибудь временную папку. Нас интересует файлик MinEdLauncher.exe
3. Открываем проводник и копируем его в папку где установлена игра, обычно это внутри подпапок стима:

4. Для верности запускаем его один раз на исполнение. Обычно это выдает ошибку, но при этом создается папка настроек, которая понадобится в дальнейшем.
5. Топаем в проводнике в папку настроек, созданную на предыдущем этапе:



6. Заменяем settings.json на этот:

7. Открываем клиент стим топаем в библиотеку и щелкаем правой кнопкой по ярлыку элиты. В выпавшем меню находим параметры запуска и прописываем там строку:
cmd /c "MinEdLauncher.exe %command% /autorun /autoquit /EDH4" Закрываем окно настроек.



8. Теперь запускаем игру из стима, кликая на "играть".
9. Будет запущена версия 4.0. 
10. Если захотите играть в обычном режиме и вместо использования стороннего лаунчера захочите запустить стандартный фронтировский, удалите cmd /c "MinEdLauncher.exe %command% /autorun /autoquit /EDH4" из свойств элиты в стиме или пропишите там параметры запуска нужного дополнения как это написано в описании тут: https://github.com/rfvgyhn/min-ed-launcher#arguments
На этом всё. Удачных полетов!
