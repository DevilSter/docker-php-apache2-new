## Настройка XDebugger

Сначала настроим путь до интерпретатора РНР, для этого в настройках 
на скрине ниже

![Шаг 1](./docimg/xd1.png)

тыркаем кнопку около CLI Interpreter 

![Шаг 2](./docimg/xd2.png)

В открывшемся окне нажимаем плюсик 

![Шаг 3](./docimg/xd3.png)

Откроется новое окошко. Там выбираем радио-бутон Docker и если 
Server будет пусто - то New ну и там Docker (там думаю разберетесь)

![Шаг 4](./docimg/xd4.png)

В итоге должно получитья что-то типа такого

![Шаг 5](./docimg/xd5.png)

Нажимаете ОК и обновится информация о РНР. Появится третья строчка 
PATH Mappings, нажимаете три точки и в открывшемся окошке 
добавляете маппер на ваши рабочие файлы

![Шаг 6](./docimg/xd7.png)

Далее идет в настройки дебагера как на скрине ниже. Меняете только 
одно - ***Host*** - его берете из вашего ENV файла, который вы 
создавали в самом начале из шаблона 

![Шаг 7](./docimg/xd6.png)

Ну и на вкладке Server делаете настройки как ниже и 
маппите файлы на хосте в директорию в докер контейнере

![Шаг 8](./docimg/xd8.png)