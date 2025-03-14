# Вклад

## Руководство по участию в разработке UPKGT

### Содержание

1. Начало работы
2. Правила участия
3. Процесс разработки
4. Стиль кода
5. Тестирование
6. Документация

### Начало работы

#### Подготовка окружения

```bash
# Клонирование репозитория
git clone https://github.com/AnmiTaliDev/upkgt.git
cd upkgt

# Установка зависимостей
go mod download

# Сборка проекта
./build.sh
```

#### Структура проекта

```
upkgt/
├── cmd/            # Точки входа
├── internal/       # Внутренний код
├── pkg/           # Публичные пакеты
└── docs/          # Документация
```

### Правила участия

#### Процесс внесения изменений

1. Создайте issue с описанием изменений
2. Обсудите предлагаемые изменения с сообществом
3. Сделайте fork репозитория
4. Создайте ветку для изменений
5. Внесите изменения
6. Создайте pull request

#### Правила оформления коммитов

```
тип(область): краткое описание

Подробное описание изменений
```

Типы коммитов:

* feat: новая функциональность
* fix: исправление ошибки
* docs: изменения в документации
* style: форматирование кода
* refactor: рефакторинг
* test: добавление тестов
* chore: обслуживание кода

#### Code Review

* Каждый PR должен быть проверен минимум одним разработчиком
* Код должен соответствовать стилю проекта
* Должна быть обновлена документация

### Процесс разработки

#### Ветки

```bash
# Создание ветки для фичи
git checkout -b feature/name

# Создание ветки для исправления
git checkout -b fix/name

# Создание ветки для документации
git checkout -b docs/name
```

#### Рабочий процесс

1. Синхронизация с основной веткой
2. Создание новой ветки
3. Внесение изменений
4. Обновление документации
5. Создание PR

### Стиль кода

#### Форматирование

```bash
# Форматирование кода
go fmt ./...

# Проверка стиля
go vet ./...
```

#### Правила именования

* Пакеты: короткие существительные
* Функции: глаголы
* Переменные: существительные
* Константы: ВЕРХНИЙ\_РЕГИСТР
* Интерфейсы: существительные

### Тестирование

#### Модульные тесты

```bash
# Запуск всех тестов
go test ./...

# Запуск конкретного теста
go test ./pkg/name -run TestName

# Запуск с покрытием
go test -cover ./...
```

### Документация

#### Правила документирования

* Каждый публичный API должен быть документирован
* Примеры использования обязательны
* Документация должна быть на русском языке
* Обновляйте CHANGELOG.md

Примечания:

* Следите за обновлениями в основном репозитории
* Задавайте вопросы в GitHub Discussions
* Сообщайте о проблемах через GitHub Issues
