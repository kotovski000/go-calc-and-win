# Дебаггинг через интерфейс VSCode

## Цель
Освоение процесса отладки кода на языке Go с использованием интегрированного отладчика в Visual Studio Code (VSCode) для выявления и исправления ошибок в мини-игре «Рассчитай и победи!».

## Шаги
1. Создан файл go.mod с помощью команды go mod init go-calc-and-win.
2. Создан файл launch.json с конфигурацией для запуска пакета Go и добавлен параметр "console": "integratedTerminal", который позволяет при отладке использовать терминал VSCode для ввода нужных команд в процессе игры.
3. Установлена точка останова (англ. breakpoint) на строке userTotalAttack := getUserAttack().
4. Запущен отладчик, что позволило пошагово пройти код и выявить ошибку в строке total += 1.
5. Ошибка была исправлена путём замены total += 1 на total += attackValue.