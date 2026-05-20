<!--appdeploy-->
# Развертка приложения (если backend - Node.js)
### Обновление пакетов
```bash
sudo apt update && sudo apt upgrade -y
```
## Установка Node.js (LTS версия)
```bash
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -  
sudo apt install -y nodejs
```
### Проверка установки
```bash
node --version  
npm --version
```
> Должно показать v20.x.x и 10.x.x
## Копирование приложения на сервер
### Создание директории для приложения
```bash
mkdir -p ~/myapp
cd ~/myapp
```
> Если код в Git-репозитории, то:
```bash
git clone ваш-репозиторий.git
```
> Если нет, то вы сами создаете структуру для работы
>> Я для примера сам создал структуру и сейчас буду двигаться по ней
### Настройка backend
```bash
# Переходим в папку бэкенда
cd ~/myapp/todo-app/backend
# Устанавливаем зависимости
npm install
# Проверяем файл .env
nano .env  # Отредактируйте, если нужно
```
