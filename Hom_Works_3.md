# **Hom works**

* Составить инструкию пользования Git Bash
* Вствить изображение Git
* Приложить фото с конфликтом между ветками

## **_Инструкция по терминологии Git и работа с репозиторием_**

### **Оглавление**

1. _Что такое Git_
2. _Что такое Visual Studio Code(VSC)
3. _Репозиторий_
4. _Команды управления Git_
5. _Работа с изображением_

 # 1. Что же такое Git Bash ?

 * Git Bash — это приложение для сред Microsoft Windows, эмулирующее работу командной строки Git. Bash — аббревиатура от Bourne Again Shell. Оболочка (Shell) представляет собой приложение терминала для взаимодействия с операционной системой с помощью письменных команд.

 **Установка Git** -
Прежде чем использовать Git, вы должны установить его на своём компьютере. Даже если он уже установлен, наверное, это хороший повод, чтобы обновиться до последней версии. Вы можете установить Git из собранного пакета или другого установщика, либо скачать исходный код и скомпилировать его самостоятельно.

# 2. Visual Studio Code (VS Code) 

**Visual Studio Code** (VS Code)— это редактор кода для разных языков программирования. Он относительно немного весит, гибкий и удобный. В нем можно писать, форматировать и редактировать код на разных языках.

**С VS Code** - работают программисты на разных языках. Например, им активно пользуются веб-разработчики, пишущие на HTML/CSS, JavaScript, PHP. Но редактор поддерживает намного большее количество языков: Python, Go, Ruby, C#, TypeScript и так далее. Он работает и с расширениями и фреймворками для популярных языков — например, с React JS и Vue.js, с языками стилей SCSS и LESS, которые дополняют CSS.

**_Для чего нужен VS Code_**

* VS Code позволяет легко писать, форматировать и редактировать код на разных языках. С его помощью можно быстро создать проект и структуру файлов в нем, он подсвечивает синтаксис кода и помогает автоматически править ошибки. В нем есть возможности для отладки и запуска кода на некоторых языках.

# 3. Репозиторий

__Что такое репозиторий Git?__

* Репозиторий — это все файлы, находящиеся под контролем версий, вместе с историей их изменения и другой служебной информацией.

Репозиторий Git можно создать, либо выбрав любую папку на компьютере, либо клонировав себе уже существующий репозиторий, например у работодателя.

__Где хранится репозиторий?__

Существуют разные способы хранения и использования репозитория: выделяют локальные, централизованные и распределенные системы контроля версий.

В локальных системах контроля версий репозиторий хранится и используется на одном устройстве, но работать с такой системой может только один разработчик. В случае централизованной системы репозиторий хранится на одном сервере.

* Лучше  было вчера и завтра а сегодня очень трудно всего для большого количества разработчиков подходят распределенные системы контроля версий, к которым относится и Git. Такая система представляет собой облачное хранилище: каждый пользователь хранит на своем устройстве весь репозиторий целиком, и по мере изменения репозитории синхронизируются.

# 4. Команды Git

**Git** сегодня - это очень популярная система контроля версий. Поэтому шпаргалка по Git, состоящая из основных команд - это то, что может вам пригодиться.

**_Шпаргалка по основным командам_**

__*git add*__

Команда git add добавляет содержимое рабочей директории в индекс (staging area) для последующего коммита. По умолчанию git commit использует лишь этот индекс, так что вы можете использовать git add для сборки слепка вашего следующего коммита.

__*git status*__

Команда git status показывает состояния файлов в рабочей директории и индексе: какие файлы изменены, но не добавлены в индекс; какие ожидают коммита в индексе. Вдобавок к этому выводятся подсказки о том, как изменить состояние файлов.

__*git diff*__

Команда git diff используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между вашей рабочей директорией и индексом (собственно git diff), разница между индексом и последним коммитом (git diff --staged), или между любыми двумя коммитами (git diff master branchB).

__*git difftool*__

Команда git difftool просто запускает внешнюю утилиту сравнения для показа различий в двух деревьях, на случай если вы хотите использовать что-либо отличное от встроенного просмотрщика git diff.

__*git commit*__

Команда git commit берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.

__*git reset*__

Команда git reset, как можно догадаться из названия, используется в основном для отмены изменений. Она изменяет указатель HEAD и, опционально, состояние индекса. Также эта команда может изменить файлы в рабочей директории при использовании параметра --hard, что может привести к потере наработок при неправильном использовании, так что убедитесь в серьёзности своих намерений прежде чем использовать его.

__*git rm*__

Команда git rm используется в Git для удаления файлов из индекса и рабочей директории. Она похожа на git add с тем лишь исключением, что она удаляет, а не добавляет файлы для следующего коммита.

__*git mv*__

Команда git mv — это всего лишь удобный способ переместить файл, а затем выполнить git addдля нового файла и git rm для старого.

__*git clean*__

Команда git clean используется для удаления мусора из рабочей директории. Это могут быть результаты сборки проекта или файлы конфликтов слияний.

**_Шпаргалка по ветвлению и слиянию_**

__*git branch*__

Команда git branch — это своего рода “менеджер веток”. Она умеет перечислять ваши ветки, создавать новые, удалять и переименовывать их.

__*git checkout*__

Команда git checkout используется для переключения веток и выгрузки их содержимого в рабочую директорию.

__*git merge*__

Команда git merge используется для слияния одной или нескольких веток в текущую. Затем она устанавливает указатель текущей ветки на результирующий коммит.

__*git mergetool*__

Команда git mergetool просто вызывает внешнюю программу слияний, в случае если у вас возникли проблемы слияния.

__*git log*__

Команда git log используется для просмотра истории коммитов, начиная с самого свежего и уходя к истокам проекта. По умолчанию, она показывает лишь историю текущей ветки, но может быть настроена на вывод истории других, даже нескольких сразу, веток. Также её можно использовать для просмотра различий между ветками на уровне коммитов.

__*git stash*__

Команда git stash используется для временного сохранения всех незакоммиченных изменений для очистки рабочей директории без необходимости коммитить незавершённую работу в новую ветку.

__*git tag*__

Команда git tag используется для задания постоянной метки на какой-либо момент в истории проекта. Обычно она используется для релизов.

**Шпаргалка по совместной работе и обновлению проектов**

Не так уж много команд в Git требуют сетевого подключения для своей работы, практически все команды оперируют с локальной копией проекта. Когда вы готовы поделиться своими наработками, всего несколько команд помогут вам работать с удалёнными репозиториями.

__*git fetch*__

Команда git fetch связывается с удалённым репозиторием и забирает из него все изменения, которых у вас пока нет и сохраняет их локально.

__*git pull*__

Команда git pull работает как комбинация команд git fetch и git merge, т.е. Git вначале забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой.

__*git push*__

Команда git push используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.

__*git remote*__

Команда git remote служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например "origin", так что вам не придётся забивать голову всякой ерундой и набирать её каждый раз для связи с сервером. Вы можете использовать несколько удалённых репозиториев для работы и git remote поможет добавлять, изменять и удалять их.

__*git archive*__

Команда git archive используется для упаковки в архив указанных коммитов или всего репозитория.

__*git submodule*__

Команда git submodule используется для управления вложенными репозиториями. Например, это могут быть библиотеки или другие, используемые не только в этом проекте ресурсы. У команды submodule есть несколько под-команд — add, update, sync и др. — для управления такими репозиториями.

**_Шпаргалка по осмотру и сравнению_**

__*git show*__

Команда git show отображает объект в простом и человекопонятном виде. Обычно она используется для просмотра информации о метке или коммите.

__*git shortlog*__

Команда git shortlog служит для подведения итогов команды git log. Она принимает практически те же параметры, что и git log, но вместо простого листинга всех коммитов, они будут сгруппированы по автору.

__*git describe*__

Команда git describe принимает на вход что угодно, что можно трактовать как коммит (ветку, тег) и выводит более-менее человекочитаемую строку, которая не изменится в будущем для данного коммита. Это может быть использовано как более удобная, но по-прежнему уникальная, замена SHA-1.

**_Шпаргалка по отладке_**

В Git есть несколько команд, используемых для нахождения проблем в коде. Это команды для поиска места в истории, где проблема впервые проявилась и собственно виновника этой проблемы.

__*git bisect*__

Команда git bisect — это чрезвычайно полезная утилита для поиска коммита в котором впервые проявился баг или проблема с помощью автоматического бинарного поиска.

__*git blame*__

Команда git blame выводит перед каждой строкой файла SHA-1 коммита, последний раз менявшего эту строку и автора этого коммита. Это помогает в поисках человека, которому нужно задавать вопросы о проблемном куске кода.

__*git grep*__

Команда git grep используется для поиска любой строки или регулярного выражения в любом из файлов вашего проекта, даже в более ранних его версиях.

Если вы только начинаете работать с Git, или переходите на Git с другой СКВ, то такая шпаргалка может вам очень пригодиться.

# 5. _Работа с изображением_


* __! [alt text] (example.com/logo.png)__

Как добавить картинку в readme на GitHub
Грузим картинки на GitHub, желательно в отдельный каталог, например screnshoots . Лучше грузить скрины в сам репозиторий, хотя GitHub позволяет вставку картинок и с других сайтов.
Добавляем следующий код в Hom_Works_3.md : ! [Описание] (http(s)://адрес_картинки.png(jpg , png , т.д.))

![Hello World](data:image/png;base64,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) 

# The End 
*thanks for being with us*