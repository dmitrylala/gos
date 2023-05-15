# Билеты к ГОСам

Здесь представлены билеты для подготовки к ГОСам факультета ВМК МГУ, первого потока.

## Локальная сборка

Компиляция файла main_small.tex в Overleaf с бесплатным аккаунтом не срабатывает, отнимает слишком много времени.
Поэтому добавлена возможность компилировать исходники локально с помощью Makefile.

### Сборка под Ubuntu/Debian

```console
# Установка зависимостей
sudo apt-get install -y texlive-bibtex-extra

# Доступные команды в Makefile (warning: make clean не удаляет pdf-ки)
make help
```

Компиляция pdf из исходников, в качестве target указывается main_big или main_small
```console
make compile target=main_big
```
