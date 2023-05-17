# Билеты к ГОСам

Здесь представлены билеты для подготовки к ГОСам факультета ВМК МГУ, первого потока.

## Локальная сборка

Компиляция файла main_small.tex в Overleaf с бесплатным аккаунтом не срабатывает, отнимает слишком много времени.
Поэтому добавлена возможность компилировать исходники локально с помощью Makefile.

### Зависимости Ubuntu/Debian

```console
# Установка зависимостей
sudo apt-get install -y texlive-bibtex-extra
```

### Зависимости под mac

- Можно скачать [MacTex](https://tug.org/mactex/) (весит много)
- Либо через brew, но все пакеты надо ставить вручную

```console
brew install basictex
brew install --cask tex-live-utility
# Обновить терминал
# Через tex-live-utility ставить пакеты
```

## Доступные команды в Makefile
```console
# Вывод списка доступных команд
make help

# Очистка временных файлов, создающихся в процессе компиляции
# Warning: make clean не удаляет pdf-ки
make clean

# Компиляция pdf из исходников, в качестве target указывается main_big или main_small
make compile target=main_big
```
