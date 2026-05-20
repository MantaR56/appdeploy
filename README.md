> appdeploy
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
