# A-Bot_GUI DeltaController.exe crafted by TomBishop
GIU Controller for A-Bot https://github.com/dpcwee/abot

!!!Внимание - читаем всё!!!
1. Controller не умеет влиять на работу бота: торгов, настроек и всему, что может навредить Вашему Депо, по простому софт сокращает несколько действий человека в одну кнопку
2. Не стоит закрывать бота в момент когда идёт активность торгов - это может привести к сбое в базе данных бота

# Условия:
0. Windows 10
1. Фаил DeltaController.exe должен находится в папке с ботом
2. Запуск DeltaController.exe от имени Администратора, т.к окно бота игнорирует комаду на закрытие если она не от Администратора
3. Версия бота должна быть с Дельтой в title в торгах, уточняйтя в телеграм у Андрея, или запустите торги и проверьте дублируется ли Дельта в заголовок окна.
4. Имена файлов бота должны быть: A-Bot-BTC.exe и A-Bot-USDT.exe

# Что умеет DeltaController:
1. Вверху 2 радиобокса - выбор версии бота для контроля.
2. Кнопка Start Bot - запускает бота выбранного в пункте 1, если бот уже запущен - всплывет предупреждение
3. Кнопка Start trade - за человека выполняет команду -s в терминале бота, в случе если бот уже в торговле -всплывет предупреждение PS: Нажимайте её только если бот находится в лобби
4. Кнопка Close Bot - закрывает выбранного в пункте 1 бота.
5. Подраздел Restart Every: - 3,6,12 часов пока не доступны ибо безусловное закрытие бота в момент активности торгов может вызвать сбой базы бота, у меня так и произошло ))
6. Radiobutton AUTO - После нажатия на Кнопку Start Automatics: Запускает каждые 10 мин анализатор изменения Дельты - первый запрос Δ0 становится Опорным, далее в течении минуты, каждые 3 секунды снова запрашивает Δ1, которая становится Контрольной и если Контрольная Δ1 за 20 проверок совпадает с Опорной Δ0 - автоматика выгружает Бота, через 5сек его запускает снова, и еще через 10сек отправляет бота в торги и все это без участия человека.
7. Кнопка Reload - Перезапускает окно Контроллера
8. Кнопка Close - Закрывает окно Контроллера
9. Cycles: - счетчки перезапуска бота
10. Кнопка A-Bot website - открывает в браузере страничку A-Bot на GitHub - https://github.com/dpcwee/abot
11. Кнопка GUI Controller website - открывает в браузере страничку GIU Controller на GitHub - https://github.com/TomBishop-Auto/A-Bot_GUI
12. Кнопка Donate website - открывает в браузере страничку с риквизитами, если появилось жгучее желание поддержать мну. 

# Donate

1. BNB BEP20 (BSC) - 0x1cb64ae704aa04a979b2096ea9d539660a8c04fe
2. USDT TRC20      - TNdwdecdCGboB2ede7TBwxTqNkwjVEfEQQ
3. BTC             - 1Cftcodfw4NLXwrYi4svYnofHvkuhdF2Jj
4. ETH ERC20       - 0x1cb64ae704aa04a979b2096ea9d539660a8c04fe
