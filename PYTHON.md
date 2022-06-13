# FAQ_Python

## Обновление пакетов в окружении или на глобальном уровне

`pip list --outdated --format=freeze | grep -v '^\-e' | cut -d = -f 1 | xargs -n1 pip install -U` работает на Linux
