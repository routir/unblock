Единые списки для Clash(DOMAIN-SUFFIX), PBR, Podkop, Ruantiblock для обхода блокировок через WARP на территории РФ.

Включают в себя популярные сайты, онлайн-кинотеатры, торрент-трекеры

---
- Discord - ОК (в папке services есть голосовые подсети)

- Facebook - OK

- Instagram - ОК

- TikTok - OK >>>может быть заблокирован-зависит от провайдера<<<

- X.COM(twitter) - OK

- Youtube - ОК >>>

<details><summary>YOUTUBE</summary>
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

P.S. в начале 2025 YouTube начал показывать многочасовую рекламу(для борьбы с резками) и проблема 59 секунды исчезла.
</details>

<details><summary>VIBER</summary>
заблокированы viber.com rakuten.com и подсети амазона

В папку services добавлен список [viber-ip-de.lst](https://raw.githubusercontent.com/routir/unblock/refs/heads/main/services/viber-ip-de.lst) с проверенными CIDR

Некоторые подсети разрешаются через s3.amazonaws.com , в папку servivces добавлен тестовый список [viber-ip-test.yaml](https://raw.githubusercontent.com/routir/unblock/refs/heads/main/services/viber-ip-test.yaml) с доменом amazonaws.com , а соответствующие CIDR закомментированы

При использовании Вайбера через прокси будьте осторожны, т.к. он поднимает множество соединений на разных портах, на которые может падать и торрент-трафик. Лучше всего направлять через WARP или нечувствительные прокси.
</details>



---
Списки Clash, Podkop, Ruantiblock отсортированы по категориям для лучшего понимания. 


Основано на репозиториях:

https://github.com/itdoginfo/allow-domains

https://github.com/dartraiden/no-russia-hosts

https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash

https://github.com/v2fly/domain-list-community/tree/master/data

https://iplist.opencck.org/

https://github.com/Ground-Zerro/DomainMapper

https://github.com/GhostRooter0953/discord-voice-ips

https://github.com/shvchk/unblock-net/blob/main/lists/ru-blocked.list

https://github.com/zapret-info/z-i

https://core.telegram.org/resources/cidr.txt

https://ip-ranges.amazonaws.com/geo-ip-feed.csv
