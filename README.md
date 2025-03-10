### Hexlet tests and linter status:
[![Actions Status](https://github.com/Daria-Kop/php-project-48/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/Daria-Kop/php-project-48/actions)
[![Maintainability](https://api.codeclimate.com/v1/badges/95e8c531d059b0ac8203/maintainability)](https://codeclimate.com/github/Daria-Kop/php-project-48/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/95e8c531d059b0ac8203/test_coverage)](https://codeclimate.com/github/Daria-Kop/php-project-48/test_coverage)

# Difference Calculator (Вычислитель отличий)

## О проекте

Вычислитель отличий – программа, определяющая разницу между двумя структурами данных. Это популярная задача, для решения которой существует множество онлайн-сервисов, например: http://www.jsondiff.com/. Подобный механизм используется при выводе тестов или при автоматическом отслеживании изменении в конфигурационных файлах.  
  
Возможности утилиты:
- Поддержка разных входных форматов: yaml и json
- Генерация отчета в виде plain text, stylish и json

## Системные требования

- Linux, MacOS
- PHP 8.3
- Composer 2.6.6

## Инструкция по установке

Выполните последовательно следующие действия:

1. Клонируем репозиторий:
    
    ```bash
    git clone git@github.com:Daria-Kop/php-project-48.git difference-calculator
    ```
    
2. Переходим в директорию проекта:
    
    ```bash
    cd difference-calculator
    ```
    
3. Устанавливаем зависимости:
    
    ```bash
    make install
    ```
    
4. Добавляем права на исполнение файлов в директории bin:
    
    ```bash
    chmod +x ./bin/*
    ```

## Запуск программы

Команды для запуска:

- `./bin/gendiff -h` — вывод справки.
- `./bin/gendiff --format stylish file1.json file2.json` — сравнение файлов json в формат stylish.
- `./bin/gendiff --format stylish file1.yml file2.yml` — сравнение файлов yaml в формат stylish.
- `./bin/gendiff --format plain file1.json file2.json` — сравнение файлов json в формат plain.
- `./bin/gendiff --format plain file1.yml file2.yml` — сравнение файлов yaml в формат plain.
- `./bin/gendiff --format json file1.json file2.json` — сравнение файлов json в формат json.
- `./bin/gendiff --format json file1.yml file2.yml` — сравнение файлов yaml в формат json.
- `./bin/gendiff file1.json file2.json` — если не указать формат, то stylish будет по умолчанию.

## Демонстрация

#### Вывод справки
[![asciicast](https://asciinema.org/a/W5xFnM1k43orI0VKgK5OpX9AJ.svg)](https://asciinema.org/a/W5xFnM1k43orI0VKgK5OpX9AJ)
  
#### Пример сравнения файлов json в формат stylish
[![asciicast](https://asciinema.org/a/GfF6983UgE6V9Bw92qNnD9KiY.svg)](https://asciinema.org/a/GfF6983UgE6V9Bw92qNnD9KiY)
  
#### Пример сравнения файлов yaml в формат stylish
[![asciicast](https://asciinema.org/a/oJTvWcADNMcJC8E9VMAr2gi73.svg)](https://asciinema.org/a/oJTvWcADNMcJC8E9VMAr2gi73)

#### Пример сравнения файлов json с вложенной структурой в формат stylish
[![asciicast](https://asciinema.org/a/arnWjBX7yeQWK4Il5KgyH1bOm.svg)](https://asciinema.org/a/arnWjBX7yeQWK4Il5KgyH1bOm)

#### Пример сравнения файлов yaml с вложенной структурой в формат stylish
[![asciicast](https://asciinema.org/a/tnzft2QfYi8ZcTNUXFrMdnFC6.svg)](https://asciinema.org/a/tnzft2QfYi8ZcTNUXFrMdnFC6)

#### Пример сравнения файлов json с вложенной структурой в формат plain
[![asciicast](https://asciinema.org/a/r0g5mmchD9GPhYhvXCTOCNbxq.svg)](https://asciinema.org/a/r0g5mmchD9GPhYhvXCTOCNbxq)

#### Пример сравнения файлов yaml с вложенной структурой в формат plain
[![asciicast](https://asciinema.org/a/5HTdtE9HHjVHdDGeGaqtMrZfY.svg)](https://asciinema.org/a/5HTdtE9HHjVHdDGeGaqtMrZfY)

#### Пример сравнения файлов json с вложенной структурой в формат json
[![asciicast](https://asciinema.org/a/etOAkRQBJPBpmug9uQ17bUu4k.svg)](https://asciinema.org/a/etOAkRQBJPBpmug9uQ17bUu4k)

