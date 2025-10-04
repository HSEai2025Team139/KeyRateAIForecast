[![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?logo=jupyter&logoColor=white)](https://jupyter.org)
[![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Beautiful Soup](https://img.shields.io/badge/-Beautiful_Soup-1E407D?logo=beautifulsoup&logoColor=white)](https://www.crummy.com/software/BeautifulSoup/)
[![Requests](https://img.shields.io/badge/-Requests-FF9900?logo=requests&logoColor=white)](https://docs.python-requests.org/)
[![CatBoost](https://img.shields.io/badge/-CatBoost-F491A3?logo=catboost&logoColor=white)](https://catboost.ai)
[![Airflow](https://img.shields.io/badge/-Apache_Airflow-017CEE?logo=apache-airflow&logoColor=white)](https://airflow.apache.org)
[![WordCloud](https://img.shields.io/badge/-WordCloud-4B72C8?logo=python&logoColor=white)](https://amueller.github.io/word_cloud/)
[![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org)
[![Transformers](https://img.shields.io/badge/-Transformers-792EE5?logo=huggingface&logoColor=white)](https://huggingface.co/transformers)
[![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io)
[![MLflow](https://img.shields.io/badge/-MLflow-00ACED?logo=mlflow&logoColor=white)](https://mlflow.org)
[![DVC](https://img.shields.io/badge/-DVC-00A3E0?logo=data-version-control&logoColor=white)](https://dvc.org)
[![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)](https://github.com/features/actions)

Классификатор пресс-релизов ЦБ с предсказанием будущей ключевой ставки

---

## Команда проекта

| ФИО              | никнеймы в Telegram | никнеймы в GitHub/GitLab |
|------------------|-----|--------------------------|
| Чмутенко Елена   | @helenBg | LinkiChmu                |
| Фадеев Глеб            | @ganbei | notglebatall                 |

## Куратор проекта

ФИО: [ Гераськина Надежда ]  
Контакты: [ @Nadya_Gera ]

---

## План работы

### Roadmap (KeyRateAIForecast) — завершение в апреле 2026

| Месяц | Задачи                                                                                                                                                                                                                                                                                                                                          |
|-------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Сентябрь 2025** | • Создать GitHub-организацию и репозиторий<br>• Настроить ветки `main` и `dev`, правила PR<br>• Заполнить README (описание, цель, команда, roadmap)<br>•  Договориться о комментариях к веткам/коммитам                                                                                                                                         |
| **Октябрь 2025** | • Сбор пресс-релизов ЦБ и макроданных (парсер на Selenium)<br>• Разметка таргета {-1, 0, +1}<br>• Предобработка текстов: нижний регистр, удаление пунктуации, извлечение би-/триграмм (re, nltk)<br>• Визуализация частоты слов (WordCloud)<br>• Токенизация (nltk)<br>• Лемматизация (pymorphy3)<br>• Первые бейзлайны: TF-IDF + логрег/SVM, CatBoost                                                                                                                           |
| **Ноябрь 2025** | • Расширенные фичи: sentiment, эмбеддинги (ruBERT)<br>• Подготовка табличных фичей (ВВП, CPI, лаги)<br>• Построение и сравнение бейзлайнов (CatBoost, LightGBM)                                                                                                                                     |
| **Декабрь 2025** | • Разработка моделей:<br> 1) TF-IDF + логрег/SVM, CatBoost (baseline)<br> 2) CatBoost/LightGBM (табличные фичи + агрегаты текста)<br> 3) LSTM/BiLSTM (последовательная модель на тексте)<br> 4) ruBERT/RuRoBERTa (fine-tuning)<br>• Запуск первых экспериментов по каждому направлению |
| **Январь 2026** | • Завершить разработку моделей<br>• Настройка гиперпараметров<br>• Интерпретация результатов (SHAP, attention)<br>• Сравнение моделей, выбор лучшего ансамбля                                                                                                                                                                                 |
| **Февраль 2026** | • Разработка API (FastAPI)<br>• MVP веб-приложения (Streamlit)<br>• Опционально — Telegram-бот<br>• Подключение трекинга экспериментов (MLflow/W&B)                                                                                                                                                                                             |
| **Март 2026** | • Настройка CI/CD (GitHub Actions)<br>• Мониторинг данных и качества<br>• Автоматизация ретренинга (раз в квартал)<br>• Подготовка статьи/поста для Хабра                                                                                                                                                                                       |
| **Апрель 2026** | • Финальная презентация<br>• Полный отчёт (данные, модели, метрики, вклад)<br>• Демонстрация веб-сервиса/бота<br>• Итоги: сравнение моделей, уроки                                                                                                                                                                                              |


###  Цель проекта

Разрабока системы анализа текстов пресс-релизов Центрального банка для прогнозирования динамики ключевой ставки
