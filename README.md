# Классификация гистологических изображений

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Jo6LFDLG6kpLcM6xN3QeIMwhauyrhDzX/view?usp=sharing)
## **Обзор проекта**
Данный проект представляет собой решение задачи классификации изображений гистологических срезов ткани. 

**Цели проекта:**
1. Реализация пайплайна обучения для кастомной модели (`SimpleCNN`) и предобученной модели (`FineTunedResNet`).
2. Оценка модели по метрикам: чувствительность, специфичность и точность.
3. Поддержка планировщиков скорости обучения и настройки гиперпараметров.
4. Расширенные техники аугментации данных для улучшения обобщения.
5. Автоматическое сохранение и загрузка модели, а также тестирование на нескольких наборах данных.
6. Автоматическая загрузка лучшей модели из Google Drive функцией `load()` вызываемой без аргументов.

---

## **Результаты**

1. **Производительность модели**:
   - Лучшая модель: **FineTunedResNet**
   - Точность на тестовом наборе: **0.9909**

2. **Визуализации**:
   - Матрица ошибок с расчетом чувствительности и специфичности для каждого класса.
   - Графики потерь и точности на этапах обучения и валидации.

4. **Реализованные функции**:
   - Поддержка интеграции с Google Drive для сохранения и загрузки моделей.
   - Стратифицированное разделение данных на обучающую и валидационную выборки.
   - Комплексная аугментация данных:
     - Кадрирование
     - Ротация

---





## Дополнительные реализованные опции

- #LBL1 - Валидация модели на части обучающей выборки
- #LBL2 - Автоматическое сохранение модели при обучении
- #LBL3 - Tensorboard визуализация
- #LBL4 - Валидация модели на отдельной выборке
- #LBL5 - Сохранение модели в файл и загрузка из файла
- #LBL6 - Возможность дообучения модели
- #LBL7 - Возможность использования предобученной модели
- #LBL8 - Возможность использования различных оптимизаторов
- #LBL9 - Возможность использования различных функций потерь
- #LBL10 - Возможность использования различных планировщиков lr
- #LBL11 - Early stopping
- #LBL12 - Использования различных аугментаций данных
- #LBL13 - Построение графиков обучения
- #LBL14 - Вывод confusion matrix и чувствительности/специфичности модели
- #LBL15 - В класс Dataset добавлены методы для работы с даталоадером PyTorch