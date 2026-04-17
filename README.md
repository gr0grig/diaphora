# Diaphora 3.2.1 (IDA 9.2 mod)

Модификация [Diaphora 3.2.1](https://github.com/joxeankoret/diaphora) с патчами для совместимости с IDA Pro 9.2.

## Изменения относительно оригинала

- **PyQt5 -> PySide6**: IDA 9.2 убрала PyQt5, импорты заменены на PySide6 с фолбэком на PyQt5 для старых версий.
- **idc.get_ordinal_qty()**: удалена в IDA 9.x, заменена на `get_ordinal_limit()`.
- **Recursion depth**: увеличен лимит рекурсии для алгоритма Тарьяна (SCC) на сложных CFG.
- **Compilation units**: ошибки NLTK/LFA при поиске компиляционных модулей больше не роняют весь экспорт.

## Оригинальный проект

https://github.com/joxeankoret/diaphora

Автор: Joxean Koret. Лицензия: GNU AGPL v3.
