# Vocab Trainers

Коллекция автономных HTML-тренажёров для изучения английской лексики (карточки, тесты, ввод с клавиатуры, справочник и озвучка через Web Speech API).

**Открыть на GitHub Pages:** https://wixxee.github.io/vocab-trainers/

## Доступные тренажёры

| Тема | Объём | Мобильная версия (`-mobile`) | Полная версия (`-trainer`) |
| :--- | :--- | :--- | :--- |
| **Irregular Verbs** | 185 глаголов (V1 / V2 / V3) | [irregular-verbs-mobile.html](https://wixxee.github.io/vocab-trainers/irregular-verbs-mobile.html) | [irregular-verbs-trainer.html](https://wixxee.github.io/vocab-trainers/irregular-verbs-trainer.html) |
| **Travel & Cities** | 93 слова и выражения | [travel-vocab-mobile.html](https://wixxee.github.io/vocab-trainers/travel-vocab-mobile.html) | [travel-vocab-trainer.html](https://wixxee.github.io/vocab-trainers/travel-vocab-trainer.html) |

## Особенности

- **Без бэкенда и зависимостей:** каждый тренажёр — один самодостаточный HTML-файл.
- **Сохранение прогресса:** статус изучения хранится в `localStorage` браузера и синхронизирован между мобильной и полной версией на одном устройстве.
- **4 режима тренировки:**
  - **Карточки** — 3D-переворот, свайпы на мобильной версии и горячие клавиши на десктопе.
  - **Тест** — автопереход при правильном ответе (в Irregular Verbs используется схема `2+2`: два слова, по одному верному и одному ложному варианту форм).
  - **Ввод / Письмо** — активное вспоминание с подсказками и отключённой автокоррекцией на мобильной клавиатуре.
  - **Таблица / Словарь** — поиск, режим скрытия ответов (blur) и ручная отметка выученных слов.
- **Озвучка:** ручной запуск по кнопке `🔊` (Web Speech API). На iPhone для работы звука должен быть выключен беззвучный режим (Silent Mode).

## Структура файлов

```text
vocab-trainers/
├── index.html                     # Главная страница со списком тренажёров и прогрессом
├── irregular-verbs-mobile.html    # Irregular Verbs — мобильная версия
├── irregular-verbs-trainer.html   # Irregular Verbs — полная (десктопная) версия
├── travel-vocab-mobile.html       # Travel & Cities — мобильная версия
├── travel-vocab-trainer.html      # Travel & Cities — полная (десктопная) версия
└── README.md
```
