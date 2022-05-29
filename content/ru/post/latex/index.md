---
# Documentation: https://wowchemy.com/docs/managing-content/

title: LaTeX
subtitle: Качественная система набора текста
summary: Пост про LaTeX
authors: [Garut A. I.]
tags: []
categories: []
date: 2022-05-14T14:22:56+03:00
lastmod: 2022-05-14T14:22:56+03:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

![LaTeX_logo](LaTeX_project_logo_bird.svg.png)

## Обзор

LaTeX — это программная система для подготовки документов. При написании писатель использует обычный текст, а не форматированный текст, который можно найти в текстовых процессорах «что видишь, то и получишь», таких как Microsoft Word, LibreOffice Writer и Apple Pages. Автор использует соглашения о тегах разметки, чтобы определить общую структуру документа, стилизовать текст по всему документу (например, выделить жирным шрифтом и курсивом), а также добавить цитаты и перекрестные ссылки. Дистрибутив TeX, такой как TeX Live или MiKTeX, используется для создания выходного файла (например, PDF или DVI), подходящего для печати или цифрового распространения.

LaTeX широко используется в научных кругах для обмена и публикации научных документов во многих областях, включая математику, информатику, инженерию, физику, химию, экономику, лингвистику, количественную психологию, философию и политологию. Он также играет заметную роль в подготовке и публикации книг и статей, содержащих сложные многоязычные материалы, такие как санскрит и греческий. LaTeX использует программу набора текста TeX для форматирования своего вывода и сам написан на языке макросов TeX.

LaTeX можно использовать как самостоятельную систему подготовки документов или как промежуточный формат. Например, в последней роли он иногда используется как часть конвейера для перевода DocBook и других форматов на основе XML в PDF. Система набора текста предлагает программируемые функции настольной издательской системы и широкие возможности для автоматизации большинства аспектов набора текста и настольной публикации, включая нумерацию и перекрестные ссылки на таблицы и рисунки, заголовки глав и разделов, включение графики, макет страницы, индексирование и библиографии.

Как и TeX, LaTeX начинался как инструмент письма для математиков и специалистов по информатике, но даже с самого начала своего развития он также использовался учеными, которым нужно было писать документы, содержащие сложные математические выражения или нелатинские шрифты, такие как арабский. , деванагари и китайский.

LaTeX предназначен для предоставления описательного языка разметки высокого уровня, который упрощает доступ к возможностям TeX для писателей. По сути, TeX обрабатывает макет, а LaTeX — контент для обработки документов. LaTeX включает в себя набор макросов TeX и программу для обработки документов LaTeX, и, поскольку простые команды форматирования TeX являются элементарными, он предоставляет авторам готовые команды для требований форматирования и макета, таких как заголовки глав, сноски, перекрестные ссылки и библиографии. .

## Система набора текста

LaTeX пытается следовать философии дизайна, отделяя презентацию от контента, чтобы авторы могли сосредоточиться на содержании того, что они пишут, не обращая внимания одновременно на его внешний вид. При подготовке документа LaTeX автор указывает логическую структуру, используя простые знакомые понятия, такие как глава, раздел, таблица, рисунок и т. д., и позволяет системе LaTeX обрабатывать форматирование и расположение этих структур. В результате он поощряет отделение макета от содержимого, но при этом позволяет вносить коррективы вручную, когда это необходимо. Эта концепция аналогична механизму, с помощью которого многие текстовые процессоры позволяют определять стили глобально для всего документа, или использованию каскадных таблиц стилей для оформления HTML-документов.

Система LaTeX — это язык разметки, который управляет набором текста и визуализацией и может быть произвольно расширен за счет использования базового макроязыка для разработки пользовательских макросов, таких как новые среды и команды. Такие макросы часто собираются в пакеты, которые затем можно сделать доступными для удовлетворения некоторых конкретных потребностей в наборе текста, таких как форматирование сложных математических выражений или графики (например, использование среды align, предоставляемой пакетом amsmath, для создания выровненных уравнений).

Чтобы создать документ в LaTeX, вы сначала пишете файл, скажем, document.tex, используя предпочитаемый вами текстовый редактор. Затем вы передаете свой файл document.tex в качестве входных данных для программы TeX (с загруженными макросами LaTeX), которая предлагает TeX записать файл, подходящий для просмотра на экране или печати. Этот цикл «запись-формат-предварительный просмотр» является одним из основных отличий работы с LaTeX от стиля редактирования документов «что видишь, то и получаешь» (WYSIWYG). Это похоже на известный программистам цикл код-компиляция-выполнение. Сегодня многие программы редактирования, поддерживающие LaTeX, делают этот цикл простым нажатием одной клавиши, при этом предварительный просмотр вывода отображается на экране рядом с окном ввода. Некоторые онлайн-редакторы LaTeX даже автоматически обновляют предварительный просмотр, в то время как другие онлайн-инструменты обеспечивают поэтапное редактирование на месте, смешанное с предварительным просмотром в оптимизированном едином окне.

## Сопутствующее программное обеспечение

В качестве пакета макросов LaTeX предоставляет набор макросов для интерпретации TeX. Существует много других пакетов макросов для TeX, включая Plain TeX, GNU Texinfo, AMSTeX и ConTeXt.

Когда TeX «компилирует» документ, он следует (с точки зрения пользователя) следующей последовательности обработки: Макросы → TeX → Драйвер → Вывод. Различные реализации каждого из этих шагов обычно доступны в дистрибутивах TeX. Традиционный TeX выводит файл DVI, который обычно преобразуется в файл PostScript. Совсем недавно Hàn Thế Thành и другие написали новую реализацию TeX под названием pdfTeX, которая также выводит в PDF и использует функции, доступные в этом формате. Механизм XeTeX, разработанный Джонатаном Кью, с другой стороны, объединяет современные технологии шрифтов и Unicode с TeX.

Шрифтом по умолчанию для LaTeX является Knuth's Computer Modern, который придает документам по умолчанию, созданным с помощью LaTeX, такой же отличительный вид, как и созданным с помощью простого TeX. XeTeX позволяет использовать шрифты OpenType и TrueType (то есть контурные) для выходных файлов.

Существует также множество редакторов для LaTeX, некоторые из которых являются автономными, основанными на исходном коде, а другие — онлайновыми, частично основанными на WYSIWYG. Подробнее см. в разделе Сравнение редакторов TeX.

## Совместимость и конвертеры

Документы LaTeX (*.tex) можно открыть в любом текстовом редакторе. Они состоят из обычного текста и не содержат скрытых кодов форматирования или двоичных инструкций. Кроме того, можно совместно использовать документы TeX, преобразуя файл LaTeX в формат Rich Text Format (*.rtf), XML или контейнерный формат .cls. Это можно сделать с помощью бесплатных программ LaTeX2RTF или TeX4ht. LaTeX также может быть преобразован в файлы PDF с помощью расширения LaTeX pdfLaTeX. Файлы LaTeX, содержащие текст Unicode, могут быть преобразованы в PDF-файлы с помощью пакета inputenc или с помощью расширений TeX XeLaTeX и LuaLaTeX.

HeVeA — это конвертер, написанный на Ocaml, который конвертирует документы LaTeX в HTML5. Он распространяется под лицензией Q Public License.
LaTeX2HTML — это конвертер, написанный на Perl, который преобразует документы LaTeX в HTML. Таким образом, например, научные статьи, в первую очередь набранные для печати, могут быть размещены в Интернете для онлайн-просмотра. Он находится под лицензией GNU GPL v2. Последние обновления доступны на сайте CTAN.
LaTeXML — это бесплатное общедоступное программное обеспечение, написанное на Perl, которое преобразует документы LaTeX в различные структурированные форматы, включая HTML5 (с MathML), epub (инкапсуляция HTML), jats, tei.
Pandoc — это «универсальный конвертер документов», способный преобразовывать LaTeX во множество различных форматов файлов, включая HTML5, epub, rtf и docx. Он находится под лицензией GNU GPL v2.
LaTeX стал стандартом де-факто для набора математических выражений в научных документах. Следовательно, существует несколько инструментов преобразования, ориентированных на математические выражения LaTeX, такие как преобразователи в MathML или систему компьютерной алгебры.

MathJax — это библиотека JavaScript для преобразования LaTeX в MathML, форматы изображений или HTML.
Фонд Викимедиа использует его для создания Mathoid, конвертера веб-сервисов с использованием Node.js, который преобразует математические входные данные, такие как LaTeX, в форматы MathML и изображений, включая SVG и PNG. Matoid используется в Википедии для отображения математики.
KaTeX — это библиотека JavaScript для преобразования LaTeX в HTML и MathML. Он разработан Академией Хана и является одним из самых быстрых конвертеров LaTeX в HTML.