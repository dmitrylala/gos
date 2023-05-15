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
либо скачать [MacTex](https://tug.org/mactex/) (весит много)

либо через brew, но все пакеты надо ставить вручную
```
brew install basictex
brew install --cask tex-live-utility
#обновить терминал
#через tex-live-utility ставить пакеты
```



# Доступные команды в Makefile (warning: make clean не удаляет pdf-ки)
```
make help
```

Компиляция pdf из исходников, в качестве target указывается main_big или main_small
```console
make compile target=main_big
```


