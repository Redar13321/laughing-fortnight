# Friday Night Funkin' - Twist Engine (ALPHA)

Этот проект является фанацким кастомным движком [Friday Night Funkin'](https://github.com/FunkinCrew/Funkin), ориентированный на более эффективную разработку модов и на более расширенный функционал и возможности с точки зрения процесса и визуала.

## Содержание

1. [Язык](#язык)
2. [Фреймворк](#фреймворк)
3. [TODO список](#todo-список)
4. [Реализованный функционал](#реализованный-функционал)
5. [Информация для участников проекта](#для-участников-проекта)

---

## Язык

Для разработки используется язык Haxe по следующим причинам:
- Язык является кроссплатформерным, что позваляет компилировать код под другие языки, примеру как `C++` или `JavaScript`.
- Для мододелов, до этого работающих с haxe языком, будет привычно работать с движком.

---

## Фреймворк

Используется фреймворк [Flixel](https://github.com/HaxeFlixel/flixel), который основывается на библиотеке [OpenFL](https://github.com/openfl/openfl), который основывается на библиотеке [Lime](https://github.com/openfl/lime), который использует следующие фреймвокри:
- OpenGL
- Cairo
- OpenAL

---

## TODO список

- [X] Поддержка модов
- [X] Поддержка hscript скриптов
- [ ] Поддержка lua скриптов
- [ ] Поддержка python скриптов
- [ ] Улучшение библиотек
	- [ ] Flixel
	- [ ] Openfl
	- [ ] Lime
	- [ ] HScript
- [ ] Собственные библиотеки
	- [ ] FMOD
- [ ] Чарты от 1K до 9K и более
- [ ] Поддержка кастомных наложений
- [ ] Поддержка импорта и экспорта чартов и персонажей от стороних движков
- [ ] Динамическое изменение матриц и дочерхних версий в спрайтах
- [ ] Поддержка базового 3D для спрайтов

---

## Реализованный функционал

### Поддержка модов

Игра способна на разработку своих песней, сцен, чартов, менюшек и неделей без повторного компилирования исходного кода.

### Поддержка hscript скриптов

HScript является упрощённой версии интерпретируемого языка Haxe. С помощью данной особенности, hscript позволяет манипулировать процессами игры.

### Поддержка кастомных наложений (WIP)

Обычный flixel способен выводить только `NORMAL`, `ADD`, `SUBSTRACT`, `SCREEN`, `LIGHTEN` и `DARKEN` наложения. Поэтому была сделана возможность позволить преодолеть данное ограничение и в последствии позволить на рантайме писать свои наложения через `GLSL` шейдеры.

---

## Для участников проекта:

- Майн ветка используется для показа стабильной версии
- Дев ветка используется для основной разработки
- Экспериментальная ветка используется для тестирования новых функций
- Тест ветка используется для тестирования изменений от контребьютров
- Разработка проходит внутри дев ветки
- Слияние из дев в мейн разрешается только при проверенном билде и при наличии одобрения от директоров

---

## Инфа для контребъютеров

- Не коммитить изменения без развёрнутого описания решённой проблемы
- Применяются изменения только с ветки теста.
