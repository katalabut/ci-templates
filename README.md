# Publish repo

Перейдите в текущую директорию 'helm':
```bash
cd helm
```
Упакуйте приложение с помощью Helm. Это создаст файл .tgz в текущей директории:
```bash
helm package app
```
Сгенерируйте файл индекса (index.yaml) для репозитория диаграммы:
```bash
helm repo index .
```
# Install

Добавьте репозиторий диаграммы 'app' с помощью его URL:
```bash
helm repo add app https://katalabut.github.io/ci-templates/helm/
```
