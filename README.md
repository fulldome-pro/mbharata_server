# mbharata_server

November 2023
1. static.mbharata.com возвращающая статические файлы (чтобы Арджуна мог проверять балуны и нивелировать человеческий фактор)

October 2023
1. Прототип подключения серверных переводов названий.
2. Инструкция по подготове файлов с переводами.
3. Разработки серверной части вынесены в репозиторий git и структутированы
4. nginx сконфигурирован, чтобы правильно маршрутизировать перыичные запросы (между кешем, старым сервером и новым api)
5. настроин varnish cache, храниящий локальные версии комаиксов .comics (убыстрение загрузки + в случае отказа основного сервера, серии продолжают быть доступными)
6. Доступ к зеркалу через argotunnel через сервер в регионе us
7. Мануа в репозитории по разворачиванию зеркала
8. apiProxy для отладки
9. Переписывания старого кода из устаревшего неподдерживаемого C# в node.js: device, deviceInfo, token для того чтобы приступить к реализачии задачи по индивидуальной выдачи серий


September 2023:
1. разделение dev/app для параллельной работы разработки и дизайнеров.
2. переезд ns mbharata.com на отдельный cloudflare, насткройка поддоменов с разными режимами работы
3. http/https
4. proxy/noproxy для работы с файлами >100мб
5. включением/выключение кеша
6. начат node.js api
7. разбор механизма token приложения/сервер
8. написаны инструкции по разным моментам
