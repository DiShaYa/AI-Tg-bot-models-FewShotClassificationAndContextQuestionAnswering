# Telegram Bot на Python с использованием ИИ
Этот проект представляет собой **Telegram бот**, созданный на **Python** с использованием библиотеки **TelebotApi** и **моделей машинного обучения для классификации** и **ответа на вопросы**. Бот англоговорящий и может отвечать на вопросы пользователей о космосе, используя заранее загруженный текст (context).

1. [Описание](https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/README.md#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5)
2. [Схема Работы](https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/README.md#схема-работы)
3. [Пример работы](https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/README.md#пример-работы)
4. [Инструкция по применению](https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/README.md#инструкция-по-применению)

## Описание
Бот использует две модели машинного обучения, взятые с платформы **Huggingface**:

* **Few Shot Classification**: для классификации запросов пользователей на две категории: приветствие и вопрос.
* **Context Question Answering**: для поиска ответов на вопросы пользователей в заранее загруженном тексте.

## Схема работы
<img src="https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/телеграмбот.png" width="800">

1. Пользователь отправляет запрос в Telegram бот.
2. Бот классифицирует запрос на две категории: приветствие и вопрос.
   - Если это приветствие, бот отвечает шаблонным текстом.
   - Если это вопрос, бот отправляет его в модель context question answering, которая генерирует ответ на вопрос и отправляет его пользователю.


## Пример работы
<img src="https://github.com/DiShaYa/AI-Tg-bot-models-FewShotClassificationAndContextQuestionAnswering/blob/main/Демонстрация%20работы%20бота.png" width="600">

## Инструкция по применению
1. Откройте код проекта.
2. Вставьте свой токен от вашего Telegram бота вместо -.  `token = '-'`
3. Запустите код.
4. Отправьте запросы своему телеграм боту в Telegram.
