# Business Metrics Analyzer

Учебный проект по дисциплине «Проектирование и разработка бизнесориентированного программного обеспечения».

## Бизнес-задача

Расчёт и визуализация ключевых показателей эффективности (KPI)
предприятия.

## Стек

* Python 3.10+
* pandas
* matplotlib

## Запуск

```console
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python main.py
```

Для Linux/macOS вместо команды активации PowerShell используется `source .venv/bin/activate`.

## ПЗ № 4 — проектирование архитектуры

Материалы подготовлены на основе требований и backlog этого проекта:

- [Архитектура, драйверы и обоснование решений](docs/architecture/README.md).
- [Контекст C4 L1](docs/architecture/context.png) и [контейнеры C4 L2](docs/architecture/containers.png).
- [Диаграмма компонентов](docs/architecture/components.png) и [диаграмма развёртывания](docs/architecture/deployment.png).
- [Паттерны с примерами Python](docs/architecture/patterns.md), [интерфейсы](docs/architecture/interfaces.md) и [ADR](docs/architecture/adr/).
- [Презентация на 7 слайдов](docs/architecture/pz04_presentation.pptx), [план выступления](docs/architecture/defense.md) и [ответы на 10 вопросов](docs/architecture/control_questions_pz04.md).
- [Проверка комплектности ПЗ № 4 и ссылки для сдачи](docs/architecture/assignment_checklist.md).

Документация описывает целевую архитектуру. Текущий `main.py` — консольный прототип; веб-приложение и облачное развёртывание ещё не реализованы.

Проверка учебных примеров архитектурных паттернов из корня проекта:

```console
python -m unittest discover -s docs/architecture/examples -p "test_*.py" -v
```

## Пример бизнес-задачи

Компания хранит ежемесячные данные о выручке по подразделениям.
Приложение помогает быстро увидеть среднюю выручку и рассчитать
рентабельность отдельных направлений бизнеса без ручных расчётов в Excel.

## Планируемые метрики

* Средняя выручка за период
* Рентабельность по направлениям
* Динамика выручки месяц к месяцу

Автор
Студент группы Б1123-38.03.05ба(1), ФИО Логинов Михаил.
