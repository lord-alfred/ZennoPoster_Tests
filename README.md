ZennoPoster Tests v.0.1
=======================

Автоматизированные ([регрессионные](https://ru.wikipedia.org/wiki/%D0%A0%D0%B5%D0%B3%D1%80%D0%B5%D1%81%D1%81%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%B5_%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5), [модульные](https://ru.wikipedia.org/wiki/%D0%9C%D0%BE%D0%B4%D1%83%D0%BB%D1%8C%D0%BD%D0%BE%D0%B5_%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5) и [интеграционные](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D1%82%D0%B5%D0%B3%D1%80%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%B5_%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5)) тесты для ZennoPoster. Они помогут после установки новой версии понять что сломалось.

Так как разработчики из версии в версию ломают старый функционал, прикручивая новый - уже давно в голове витала идея создать что-то такое для себя, чтобы с каждой версией не перепроверять все шаблоны - вдруг где-то что-то перестало работать. Но в итоге я понял, что такой проект лучше сделать для всех пользователей ZP.

К тому же, это поможет не только пользователям, но и разработчикам - так проще отслеживать баги. Поэтому, думаю, будет не лишним, если и они тоже будут добавлять сюда новые тестовые проекты.

Такой *публичный* репозиторий с тестами прибавит мотивации создателям этого замечтального продукта, чтоб они перед выкаткой обновлений лучше проверяли всё, что сделали. Чтобы мы, покупатели, не получали "сырую" версию программы, которая ломает все наши проекты/шаблоны.

Карта покрытия тестами
----------------------

Покрытие тестами стандартных действий (кубиков): [можно посмотреть тут](https://github.com/lord-alfred/ZennoPoster_Tests/blob/master/coverage_map.md).

Покрытие тестами встроенных C# классов/методов (ZennoLab Assemblies): пока не проводилось, стань первым, кто начнет это делать!

Запуск тестов
-------------

Для запуска тестов нужно:

1. Скачать [последний релиз](https://github.com/lord-alfred/ZennoPoster_Tests/releases) (их пока что не было, скачивайте весь репозиторий).
2. Распаковать содержимое в директорию:

    C:\zenno\ZennoPoster_Tests\

3. Добавить в ZennoPoster шаблон:

    C:\zenno\ZennoPoster_Tests\start_tests.xmlz

4. Запустить шаблон *start_tests* в ZP.

После прохождения всех тестов в окне лога в ZP будет написан путь к сгенерированному отчёту в формате HTML.

Как добавить свой тест
----------------------

Чтобы добавить свой тест (шаблон с тестом), вначале определитесь с чем он связан: со стандартными действиями (кубиками) или со встроенными C# классами/методами (ZennoLab Assemblies).

Если с кубиками, то вам нужно взять шаблон:

    test_template.xmlz

И скопировать его в нужную директорию следующим образом:

    Действия\№.Тип действия\Название действия.xmlz

Если ваш тест связан со встроенными C# классами/методами, то... я ещё не придумал как это лучше размещать :)

Контрибьютеры
-------------

После добавления своих тестов вы можете вписать имя/ник со ссылкой на свой сайт в этом разделе. Ваше имя тут останется навсегда.

Лицензия
--------

[CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/deed.ru) (Creative Commons — «Attribution-NonCommercial-ShareAlike» 3.0)

Лицензия «С указанием авторства — Некоммерческая — С сохранением условий»

Даная лицензия позволяет другим людям редактировать, поправлять и брать произведение за основу для производных в некоммерческих целях при условии, что они указывают авторство и лицензируют свои новые произведения на тех же условиях.