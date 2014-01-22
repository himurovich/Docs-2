###Виджет для плагина ManagerManager, позволяющий ограничить количество вводимых символов в TV.

mm_ddMaxLength(string $fields, string $roles, string $templates, int $length);

####Описание параметров

Название|Описание|Допустимые значения|Значение по умолчанию|Обязателен?
--------|--------|---------|-----------
fields|Поля документа (или TV), для которых необходимо применить виджет.|{comma separated string}|—|true
roles|Роли, для которых необходимо применить виждет, пустое значение — все роли.|{comma separated string}|—|false
templates|Id шаблонов, для которых необходимо применить виджет, пустое значение — все шаблоны.|{comma separated string}|—|false
length|Максимальное количество символов, которые можно ввести.|{integer}|150|false

####Примеры
Подключение виджета для TV «Slogan», ограничив количество вводимых символов до 140
	
	mm_ddMaxLength('Slogan', '', '', 140);