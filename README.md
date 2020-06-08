# Автоматическая рекомендация рефакторинга "Выделение метода" при копировании кода в IDE.


![](demo.gif)


Данный репозиторий содержит реализацию расширения для IntelliJ IDEA, который анализирует действия копирования и вставки пользователя, и автоматически предлагает совершить рефакторинг "Выделение метода" при копировании.

Структура репозитория:
* `Refactoring Experiments` содержит инструменты, необходимые для сбора данных, а также извлечения пользовательских логов операций копирования.
Для запуска сбора данных необходимо собрать проект в IntelliJ IDEA и запустить один из трех основных классов: `FalseDatasetCreator` для запуска генерации синтетических данных. `UIApplication` для запуска сбора данных посредством Refactoring Miner, `CopyLogsExtractor` для сбора логов.

* `RFTrain` содержит python-скрипты для тестирования различных моделей и построения графиков. Для запуска необходимо установить `python >=3.6`, `skipy`, `numpy`, `pandas`

* `ACP` содержит реализацию плагина. Сборка осуществляется посредством команды `./gradle buildPlugin`
Ссылка на собранный плагин: https://drive.google.com/file/d/1LXZn6s3S1ldNY-m3Yh-0QuEWc0Hj-vVv/view?usp=sharing
Для установки требуется IntelliJ IDEA 2019.2 и выше, необходимо в списке плагинов выбрать Install Plugin From Disk

Демо-видео: https://drive.google.com/file/d/1LXZn6s3S1ldNY-m3Yh-0QuEWc0Hj-vVv/view?usp=sharing

