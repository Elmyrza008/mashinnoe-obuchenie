# Машинное обучение

Учебный проект Асанова Элмырзы по дисциплине «Машинное обучение». Репозиторий содержит практики по базовым методам и темам второй половины курса.

## Структура

- `data/` — учебные наборы данных проекта.
- `notebooks/` — Jupyter Notebook с практическими работами.
- `reports/` — шаблонные требования и место для выводов по каждой работе.
- `plots/` — ранее созданные графики.
- `RULES.md` — общие правила выполнения, валидации и оформления.
- `requirements.txt` — зависимости.

## Практические работы 1–14

| № | Тема | Notebook | Отчёт |
|---:|---|---|---|
| 1 | Настройка окружения | `notebooks/practice_01_environment.ipynb` | `reports/practice_01_environment.md` |
| 2 | Разведочный анализ данных | `notebooks/practice_02_eda.ipynb` | `reports/practice_02_eda.md` |
| 3 | Предобработка и Pipeline | `notebooks/practice_03_preprocessing_pipeline.ipynb` | `reports/practice_03_preprocessing_pipeline.md` |
| 4 | Линейная регрессия | `notebooks/practice_04_linear_regression.ipynb` | `reports/practice_04_linear_regression.md` |
| 5 | Логистическая классификация | `notebooks/practice_05_logistic_classification.ipynb` | `reports/practice_05_logistic_classification.md` |
| 6 | Классификация текстов | `notebooks/practice_06_text_classification.ipynb` | `reports/practice_06_text_classification.md` |
| 7 | Случайный лес | `notebooks/practice_07_random_forest.ipynb` | `reports/practice_07_random_forest.md` |
| 8 | Градиентный бустинг | `notebooks/practice_08_gradient_boosting.ipynb` | `reports/practice_08_gradient_boosting.md` |
| 9 | Метод опорных векторов | `notebooks/practice_09_svm.ipynb` | `reports/practice_09_svm.md` |
| 10 | Кластеризация и сегментация | `notebooks/practice_10_clustering.ipynb` | `reports/practice_10_clustering.md` |
| 11 | Понижение размерности PCA | `notebooks/practice_11_pca.ipynb` | `reports/practice_11_pca.md` |
| 12 | Валидация и подбор гиперпараметров | `notebooks/practice_12_validation_tuning.ipynb` | `reports/practice_12_validation_tuning.md` |
| 13 | Многослойный персептрон | `notebooks/practice_13_mlp.ipynb` | `reports/practice_13_mlp.md` |
| 14 | Инференс и мониторинг (MLOps) | `notebooks/practice_14_mlops.ipynb` | `reports/practice_14_mlops.md` |

Работы 7–14 соответствуют темам лекций 9–16: случайный лес, бустинг, SVM, кластеризация, PCA, валидация, нейросети и внедрение.

## Установка и запуск

Требуется Python 3.10 или новее. В PowerShell из каталога репозитория выполните:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m notebook
```

Откройте нужный файл в `notebooks/` и выберите **Restart Kernel and Run All Cells**. Путь к данным рассчитан на запуск из корня репозитория или каталога `notebooks`. Практика MLOps создаёт локальные файлы в `artifacts/`; обученные модели и данные пользователей не следует публиковать.

## Отчёт

Для каждой работы используйте соответствующий файл в `reports/`: внесите таблицы/графики, конкретные результаты запуска, ответы на вопросы и ограничения. Общие требования приведены в [RULES.md](RULES.md).

## Ограничения и ответственное использование

Набор breast cancer предназначен только для учебного сравнения алгоритмов. Он не является медицинским инструментом. Кластеризация не имеет истинной разметки, если она отдельно не предоставлена. Метрики на одном train/test-разбиении имеют статистическую неопределённость. Не делайте причинных выводов из корреляций или важности признаков.
