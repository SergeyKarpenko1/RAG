# В данном репозитории представлены два проекта, реализующие системы Retrieval-Augmented Generation (RAG), каждая из которых адаптирована под конкретные бизнес-задачи.

## 1. RAG для компании Intelion

Intelion — компания, занимающаяся продажей майнингового оборудования. Данный RAG был разработан для того, чтобы сотрудники могли оперативно находить ответы на любые вопросы, касающиеся компании. База знаний включает информацию о департаментах, внутренних регламентах, правилах, философии и спектре услуг, предоставляемых компанией. Система реализована в формате чат-бота, что позволяет пользователям взаимодействовать с RAG в удобной форме.

Используемый стек технологий::

	•	Язык программирования: Python
	•	Фреймворки и библиотеки: Hugging Face, Transformers, OpenAI, FastAPI, LongChain, Chroma
	•	Модель эмбеддингов: OpenAIEmbeddings (модель: text-embedding-3-small)
	•	LLM для генерации ответов: ChatOpenAI (модель: gpt-4o-mini)

Особенности:

	•	Реализованы различные варианты промптов для улучшения контекстуализации вопросов и помощи в переформулировании запросов.
	•	Внедрены техники ReAct Docstore для взаимодействия с пользователями.
	•	Проведены эксперименты с RAG-Fusion и RRF для улучшения качества генерации ответов.

## 2. RAG для заводских работников

Второй RAG предназначен для работников завода, целью которого является ускорение поиска информации в технической литературе. Основные источники знаний включают книги, такие как “Справочник конструктора-машиностроителя” (тома 1, 2, 3) и “Допуски и посадки”. Эти материалы были представлены в формате PDF, что добавило сложности в обработке, особенно из-за наличия большого количества таблиц.

Используемый дополнительный стек технологий::

	•	Библиотека для обработки PDF: pdfplumber

Особенности:

	•	Интегрирована сложная обработка PDF-файлов с таблицами для корректного извлечения данных.
	•	Реализован функционал, аналогичный RAG для Intelion, адаптированный для работы с технической литературой.

 ## Результаты работы

Ниже представлены результаты работы чат-бота, а также примеры того, как выглядели PDF файлы из технической литературы.

RAG для компании Intelion:
![image](https://github.com/user-attachments/assets/78c67e56-01ca-432c-a1cf-32fbe271019e)

RAG для заводских работников:
![image](https://github.com/user-attachments/assets/dddbf96c-9be8-46ca-80c8-2f72764a1442)

PDF файлы:

![image](https://github.com/user-attachments/assets/cea9c0bc-4309-4f15-84be-a8656fa47072)


