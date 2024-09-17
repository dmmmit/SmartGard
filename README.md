# SmartGard 🌱

SmartGard — это сервис для садоводов, который позволяет отслеживать и контролировать уход за растениями, а также предоставляет индивидуальные рекомендации для каждого пользователя.

## Хакатон Tula-Hack 2024

Проект был разработан в рамках хакатона Tula-Hack 2024, целью которого было создание инновационных решений для поддержки и развития локальных сообществ. SmartGard ориентирован на садоводов, которые хотят оптимизировать уход за растениями с помощью современных технологий, таких как искусственный интеллект и машинное обучение.

## Проблема

Многие садоводы, особенно новички, сталкиваются с трудностями в уходе за растениями, который требует учета различных факторов: погодных условий, особенностей почвы, типа растений и их потребностей. Часто отсутствует удобная система для планирования и учета всех этих нюансов. Кроме того, советы для ухода за растениями могут быть слишком обобщенными, что не позволяет достигнуть максимальных результатов.

## Задачи

- Создать сервис, который будет предоставлять персонализированные рекомендации для ухода за растениями.
- Внедрить систему календаря, которая поможет пользователям отслеживать график ухода за растениями.
- Оптимизировать хранение данных о растениях, чтобы пользователи могли легко организовать информацию о своем саду.
- Разработать виртуального помощника, который поможет новичкам разобраться в садоводстве.

## Цели проекта

- Повысить осведомленность садоводов о правильном уходе за растениями.
- Облегчить процесс планирования ухода за растениями, создав удобную и интуитивно понятную систему календаря.
- Сделать садоводство доступным для новичков за счет внедрения виртуального помощника и советов дня.
- Предоставить более точные рекомендации за счет анализа погодных данных и типа почвы для каждого региона.

## Особенности проекта

### 1. Трехуровневая рекомендательная система

- **Анализ погоды и почвы**: Система подгружает данные о погодных условиях и состоянии почвы в указанном регионе. На основе этого предоставляются рекомендации, как эти факторы повлияют на уход за растениями каждого пользователя.
- **Общие советы и советы дня**: На главной панели пользователи могут увидеть полезные советы по уходу за садом.
- **Интеграция виртуального помощника**: Внедрение помощника через API GigaChat для поддержки пользователей на первых этапах садоводства.

### 2. Календарь садовода

В карточке каждого растения пользователи могут задать индивидуальный график ухода за растением, который будет отображаться в общем календаре, что упрощает планирование и контроль за садом.

### 3. Оптимизированное хранение

Пользователи могут создавать секции с растениями, где будет храниться вся информация о каждом растении. Эта система помогает организовать данные по каждому участку сада.

### 4. Виртуальный помощник

С помощью GigaChatAPI был создан виртуальный помощник, который помогает новичкам с рекомендациями и советами по уходу за растениями.

## Техническая реализация

### Backend:
- **Язык**: Python
- **Фреймворк**: FastAPI
- **База данных**: PostgreSQL
- **Контейнеризация**: Docker
- **Валидация данных**: Pydantic

FastAPI был использован для создания API, интегрирующего рекомендательную систему, календарь, виртуального помощника и другие функции. Swagger обеспечил связь между backend и frontend частями проекта.

### Machine Learning:
- **Фреймворки**: CatBoost, GigaChat
- **Модели**: Три модели машинного обучения, обученные на кастомном датасете, предсказывающие различные аспекты ухода за растениями (полив, удобрение, опрыскивание).
- **AI-рекомендации**: Виртуальный помощник и советы для новичков, использующие GigaChat для генерации текстов.

### Особенности ML:
- Индивидуальные рекомендации для более чем 200 типов растений.
- Внедрение AI для генерации советов дня и рекомендаций новичкам.
- Оптимизация рекомендаций с учетом данных о почве и погодных условиях.

## Стек технологий

- **Backend**: Python, FastAPI, PostgreSQL, Docker, Pydantic
- **ML**: CatBoost, GigaChat
- **Frontend**: Java Script, React, Recoil
- **Интеграции**: Swagger, GigaChatAPI

## Дизайн

Дизайн интерфейса и презентация проекта доступны на [Figma](https://www.figma.com/design/282I8JR5Zf9V4WIy5vv3id/ITUT_MISIS?node-id=129-4583&node-type=frame).

## Заключение

SmartGard объединяет передовые технологии для того, чтобы садоводство стало более доступным и эффективным. Это отличный инструмент как для новичков, так и для опытных садоводов, который упрощает уход за растениями и предлагает персонализированные советы с использованием машинного обучения.

## Авторы: 
- Уросов Дмитрий, ML engineer, 
- Тотоева Алина, designer, 
- Белов Георгий, backend-разработчик, 
- Феденко Софья, backend-разработчик, 
- Клесов Артем, frontend-разработчик
