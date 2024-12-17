# YAML CV
Этот репозиторий содержит резюме в формате [yaml-cv](https://github.com/haath/yaml-cv).

## Настройка

Установить [yq v4](https://mikefarah.gitbook.io/yq/), например:
```bash
wget https://github.com/mikefarah/yq/releases/latest/download/yq_linux_amd64 -O /usr/bin/yq &&\
    chmod +x /usr/bin/yq
```

Установить [yaml-cv](https://github.com/haath/yaml-cv):
```bash
gem install yaml-cv
```
Установить gem
```bash
sudo apt install ruby-rubygems
```

Для создания PDF-версии, требуется `wkhtmltopdf`:
```bash
brew install wkhtmltopdf
```

Установить [Taskfile](https://taskfile.dev):
```bash
sudo sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin
```

Установить [pre-commit]
```bash
sudo apt install pre-commit
```

## Использование

```bash
task --list-all
```

### Сборка

Запустить:
```bash
task build
```

### Конвертация в JSON

```bash
task json
```

### Поиск

Вывод навыков по уровню владения (`junior|middle|senior`):
```bash
task skill_by_level -- <level>
```
