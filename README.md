#### Изменение последнего коммита
git commit --amend

#### Интерактивное добавление отдельных частей файлов
git add -p

#### Интерактивное скрытие отдельных частей файлов
git stash -p

#### Интерактивный «сброс» выбранных частей файлов
git checkout -p

#### Переключение в предыдущую ветку
git checkout -

#### Сброс всех локальных изменений
git checkout 

#### Показать изменения
git diff --staged

#### Локальное переименование веток
git branch -m old-name new-name

#### Переименование веток удаленно
git push origin :old-name
git push origin new-name

#### Открыть все файлы с конфликтами одновременно
git diff --name-only --diff-filter=U | uniq  | xargs $EDITOR

#### Что изменилось?
git whatchanged --since=‘2 weeks ago’

#### Удаление файла из последнего коммита
git rm --cached <file-to-remove>
git commit --amend

#### Поиск веток
git branch --contains <commit>

#### Локальная оптимизация репозитория
git gc --prune=now --aggressive

#### Просмотреть историю коммита
git log 

#### Просмотреть, кто, что и когда изменил в my_file
git blame my_file 
