# Модификация iso-образов

## Cubic

Cubic позволяет легко модифицировать Live ISO образы дистрибутивов Debian, Ubuntu, Linux Mint.

Хороший видеоурок: https://www.youtube.com/watch?v=t1MQ1SicXj8

Исходники: https://launchpad.net/cubic

## Изучаем исходники

Изучаемая ревизия: https://bazaar.launchpad.net/~cubic-wizard/cubic/release/revision/86
Скачать ревизию: https://bazaar.launchpad.net/~cubic-wizard/cubic/release/tarball/86

Cubic написан на Python и Bash. Стартовый файл `cubic_wizard.py` и путь к нему `/usr/share/cubic`
указаны в файле `usr/share/applications/cubic.desktop`.

Исходники обильно прокомментированы и легко читаются.

Для GUI используется GTK.

Наиболее интересные файлы:
* `usr/share/cubic/commands/mount-iso`
* `usr/share/cubic/commands/unmount-iso`
* `usr/share/cubic/commands/extract-root`
* `usr/share/cubic/commands/compress-root`
* `usr/share/cubic/cubic/pages/generate_page.py` → `_get_xorriso_command()`
