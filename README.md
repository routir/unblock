
Единые списки для Ruantiblock/PBR и Clash(+.) для обхода блокировок через WARP на территории РФ.

Включают в себя популярные сайты, онлайн-кинотеатры, торрент-трекеры

---
- Discord(без голоса) - ОК (в папке services есть подсети-направлять через другой прокси)

- Facebook - OK

- Instagram - ОК

- TikTok - OK >>>может быть заблокирован-зависит от провайдера<<<

- X.COM(twitter) - OK

- VIBER - заблокированы viber.com(основные медиа), rakuten.com(звонки), rakuten-static.com и подсети amazon>>>

В папку services добавлены CIDR на Frankfurt(основной пул Европы), которые желательно пускать через другой прокси.

При звонках вызывается большой американский пул, поэтому 18.184.0.0/13, 18.192.0.0/13.

На данный момент Viber для медиаконтента использует подсети Google Cloud: 35.207.0.0/16.

Виндовый вайбер для авторизации по QR коду запрашивает 34.192.0.0/12, 52.0.0.0/15.

Все диапазоны Amazon можно посмотреть здесь https://ip-ranges.amazonaws.com/geo-ip-feed.csv

- Youtube - ОК >>>

При возниковении следующих ошибок ролики обрываются на 59 секунде

https://www.youtube.com/api/jnn/v1/GenerateIT 403 (Forbidden)

https://jnn-pa.googleapis.com/$rpc/google.internal.waa.v1.Waa/Create 403 (Forbidden)

Причин может быть несколько, начиная от бана(временного?) за использование рекламорезок(даже встроенных в браузеры фильтров отслеживания) до неполностью вырезанного ipv6, вкл/откл протокола QUIC и т.д.
Как правило, переключение на другой ВПН решает проблему. Но иногда хочется остаться на быстром ВАРПе, тогда достаточно включить jnn-pa.googleapis.com в обход через сторонний ВПН и бан автоматом снимется. Вы остаётесь территориально в РФ и ролики крутятся без рекламы. Как побочка после холодного старта долго грузится страница с видео(около 20 секунд).

Ещё один вариант - проигрывание в режиме embeded.
Ставим в хром расширение Redirector. Вбиваем настройки, сохраняем, активируем

![2024-12-23_081101](https://github.com/user-attachments/assets/c57c29db-ecac-48a8-9b38-06172da93ef2)

Ролики с трубы открываются на всё окно без комментариев и других элементов страницы, но преодолевают 59-секундный рубеж.

И последний вариант - установить расширение для смены User Agent и поменять на мобильный агент.

---
Список TEST2 отсортирован по категориям для Ruantiblock, в PBR не использовать - ломается структура


Основано на репозиториях:

https://github.com/itdoginfo/allow-domains

https://github.com/dartraiden/no-russia-hosts

https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash

https://iplist.opencck.org/

https://github.com/Ground-Zerro/DomainMapper

https://github.com/GhostRooter0953/discord-voice-ips

https://github.com/shvchk/unblock-net/blob/main/lists/ru-blocked.list

https://github.com/zapret-info/z-i

https://ip-ranges.amazonaws.com/geo-ip-feed.csv
