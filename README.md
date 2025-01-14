﻿# Logger - библиотека для журналирования/логирования событий в файл

*Проект создан в учебных целях*

* © Компьтерная Академия ШАГ. Россия (филиал Иркутск)
* Версия: 0.1 (Май 2021)

## О библиотеке

Написана на `C#` с использованием `System`, `System.IO`, `System.Threading.Tasks`
Используется асинхронная запись в файл.

### Формат записи сообщения в файл

`<дата и время> [<тип сообщения>] <сообщение>`
- `<дата и время>` - дата и время в полном формате
- `<тип сообщения>`:
    - `INFO`
    - `SUCCESS`
    - `WARNING`
    - `ERROR`

### Конструкторы

- `LogToFile(string path)`
- `LogToFile()`

### Методы

- `InfoAsync(string message)` асинхронный метод записи информационного сообщения
- `SuccessAsync(string message)`