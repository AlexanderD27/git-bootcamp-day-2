# python-test-1

Тестовая утилита пример на Python для демонстрации основных команд Git.
Для начинающих изучать Git c нуля.

## Содержание

- [Быстрый старт](#быстрый-старт)
- [Установка](#установка)
- [Использование](#использование)
- [Разработка](#разработка)
- [Пример заголовка `H3`](#пример-заголовка-h3)
- [Примеры кода (Python)](#примеры-кода-python)
- [TODO](#todo)
- [Badges](#badges)
- [Таблицы](#таблицы)
- [Лицензия](#лицензия)

## Быстрый старт

```bash
git clone git@github.com:example/python-test-1.git
cd python-test-1
python -m python-test-1 --help
```

## Установка

Зависимости: Python 3.11+. Виртуальное окружение по желанию.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Использование

Простейший сценарий:

```bash
python -m python-test-1 greet --name "Git Test"
# → Hello, Git Test!
```

<details>
<summary>Расширенный сценарий (со сворачиваемым блоком)</summary>

```bash
python -m python-test-1 greet --name "Git" --shout
# → HELLO, GIT!
```
</details>

---
### Пример заголовка `H3`
---

```text
Просто текст для примера блока text
```

---
→ [Примеры кода на Python](#примеры-кода-python)

---

---

## Примеры-кода-Python


Инициализация репозитория. Создаёт новый репозиторий в указанном каталоге:
```python
import  git
from git import Repo
new_repo = Repo.init('new_repo')
```

Клонирование репозитория. Клонирует удалённый репозиторий в новую директорию.
```python
import  git
repo = Repo.clone_from('https://github.com/username/python-test-1', '/path/to/local/directory')
```

Проверка состояния репозитория (status). Аналогично команде git status.
```python
import  git
print(repo.git.status())
```

Добавление файлов в индекс и коммит. Добавляет файлы в индекс, а затем создаёт коммит с сообщением.
```python
import  git 
repo.git.add('--all')  
repo.git.commit('-m', 'commit message from python script', author='test_user@test.com')
```

Больше примеров: → [GIT Operations with Python Scripting](https://digitalvarys.com/git-operations-with-python-scripting/#Git_Clone)


## TODO

- [x] Добавить примеры кода Python (git init, git clone, git status)
- [x] Добавить примеры кода Python (git add, git commit)
- [ ] Добавить примеры кода Python (git push, git pull)




---
## Badges

Пример:

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)


## Таблицы

Пример:

| Технология | Версия | 
|------------|---------|
| Bash    | any    | 
| Python| 3.11+     | 
 
---

## Лицензия

MIT — см. [LICENSE](LICENSE).