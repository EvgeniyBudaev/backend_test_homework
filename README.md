# backend_test_homework


GIT
fork
git clone "https://github.com/EvgeniyBudaev/имя репозитория'
git add .
git commit -m "My first commit"


Создание виртуального окружения
python3 -m venv venv


Запуск виртуального окружения проекта
В Windows:
.\venv\Scripts\activate
В macOS или Linux:
source venv/bin/activate 

Остановка виртуального окружения
deactivate 


Установка pytest и запуск тестов
pip install pytest
pytest --version 


Проверка аннотации типов
pip install mypy 
Запускаем файл утилитой mypy из директории, в которой лежит файл
mypy temp.py

Компоновщик Optional
from typing import Optional
text: Optional[str]
Компоновщик Optional аннотирует типы данных для переменных, которые могут принять два типа данных: данные определённого типа и тип None; например — str и None, bool и None.
Тип None не указывается в компоновщике Optional в явном виде

Компоновщик Union
from typing import Union
Если переменная должна принимать данные нескольких разных типов — применяют аннотацию Union. Разрешённые типы перечисляют через запятую, в квадратных скобках
х: Union[int, str]

Аннотация Any
from typing import Any
x: Any

Аннотации коллекций
from typing import Sequence, Dict, List, Tuple, Set

Псевдонимы типов
from typing import Dict, List, Union
CustomDict = Dict[str, List[Union[int, str]]]