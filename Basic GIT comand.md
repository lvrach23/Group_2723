пппп# Базовые команды GIT

## Команды терминала
* __ls__-просмотр папок в директории
> пример C:\Users>ls просмотр папок в директории Users
* __ls -a__ - расширенный просмотр, показывает все.
* __cls(clear)__ -очистить терминал
> пример PS C:\Users\lvrac\Desktop\Учебагит2> git checkout example1
Switched to branch 'example1'
PS C:\Users\lvrac\Desktop\Учебагит2> git commit -a -m "add 1 example"
On branch example1
nothing to commit, working tree clean
PS C:\Users\lvrac\Desktop\Учебагит2>
PS C:\Users\lvrac\Desktop\Учебагит2> git commit -a -m "add 1 example"
[example1 33f3220] add 1 example
 1 file changed, 5 insertions(+), 1 deletion(-)
PS C:\Users\lvrac\Desktop\Учебагит2>**cls(clear)** очистит верхние записи.
* __cd-смена__ директории(папки)
* __cd ~__- переход в корневой католог(директорию, папку)
* __cd ..__ - переход нп директорию(папку) выше
* __cd ../..__ -переход на 2 директории(папки) выше.
* __mkdir имя папки__ - создает новую папку
* __touch имя файла__ -создает новый файл. 
> пример C:\Users>touch picture.png создает файл picture.png
* __touch имя папки/имя файла__ - создает файл в указанной папке
* __cp имя оригинального файла имя копии__ - копирует файл
* __mv имя файла новое имя файла__ - йпереименовывает файл
* __echo "текс который надо добавить" > имя файла куда добляем текст__ - добляем текст в файл
* __cat имя файла__ - просмотр содержимого файла
* __rm имя файла__ - удаление файла
> C:\Users>rm picture.png удалит файл picture.png
* __rm -R__ -удаление директории(папки)


## Команды создания репозитория
* __git init__ -инициализация(создание) репозитория.
> пример C:\Users\lvrac\Desktop\Учебагит2>git init сщздает репозиторий в папке учебагит2
* __git clone__ -клонирование репозитория из удаленного в локальный.


## Команды для текущих изменений
* __git add имя файла__ - вносит файл в индекс изменений
* __git add .__ -вносит все файлы в индекс изменений


## Команды просмотра истоии изменений
* __git status__ -проверка статуса репозитория
>пример C:\Users\lvrac\Desktop\Учебагит2>git status 
* __git log__ -история комитов
* __git log --oneline__ - история комитов сокращено
* __git log --graph__ - история комитов с графическим отображением.
>C:\Users\lvrac\Desktop\Учебагит2>git log --graph вот что получиться.
![](example2.png)
* __git reflog__ - история всего
* __git diff__ - сравнивает последний комит с сохраненной только что версией документа.
* __git reset хэш комита__ - удаляет комит, но если ввести комит еще раз после удаления то но востановиться.
* __git revert хэш комита__ - отменяет действие комита


## Команды создания, ветления и слияния
* __git commit -m "коментарий изменения"__ - создает комит.
* __git commit -a -m "коментарий изменения"__ -объединяет последовательно 2 команды git add(которая вносит последние фалы которые мы изменяли), а затем git commit и вносит запись.
* __git branch__ -просмотр веток репозитория
* __git branch название ветки__ -создание новой ветки
* __git branch -d название ветки__ - удаляем ветку
* __git checkout название ветки или номер нужного комита__ -переход на новую ветку или нужный комит.
* __git checkout__ -b название ветки -переходит на ветку, если такой нет,то создает её.
* __git merge название ветки(той которая будет входить в ветку на которой находимся)__ - слияние веток.

## Команды для удаленного репозитория
* __git remote add origin сылка на удаленный репозиторий__ - синхронизация локального и удаленного репозитория, вместо origin может быть любое слово(это просто название соединения)
* __git remote -v__ проверка синхронизации
* __git push__ отправка локального репозитория на удаленныей.
* __git pull__ Вносит изменения из удаленного репозитория в текущую ветку

## Полезные ссылки.

[видеоуроки по GIT](https://youtu.be/PEKN8NtBDQ0)пп