### Простой русскоговорящий userbot для Телеграма
<p align="center">
    <a href="">
        <img src="https://raw.githubusercontent.com/Conradk10/telegram-multibot/pics/multibotby.jpg" alt="Multibot">
    </a>
	<a href="https://github.com/Conradk10/telegram-multibot/releases"><img src="https://img.shields.io/github/v/release/conradk10/telegram-multibot?include_prereleases&style=flat-square"></a>
	<a href="https://github.com/Conradk10/telegram-multibot/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Conradk10/telegram-multibot?style=flat-square"></a></br>
</br>

## 🍒 О проекте
 - Multibot представляет из себя модульного юзербота с набором различных развлекательно-инфррмационных функций а так же автоматизацию неких задач, таких как автоответчик и тд
 - Юзербот легко может дополняться с помощью написания подключаемых плагинов на языке Python

Multibot разработан для личного аккаунта Телеграм. Не для ботов (!)

Контакты:
- <a href="https://t.me/zxvghost666">Telegram</a>
- <a href="https://instagram.com/zxv.ghost666">Instagram</a>

## 🚧 Требования
- Python версии 3.6 или новее
- Telegram API ключ (https://my.telegram.org/apps)

## 📚 Библиотеки (Остальное в requirements.txt)
- <a href=https://github.com/pyrogram/pyrogram>Pyrogram 0.16.0</a><br>
- <a href=https://github.com/paramiko/paramiko>paramiko 2.7.1</a><br>
- <a href=https://github.com/giampaolo/psutil>psutil 5.6.7</a><br>
- <a href=https://github.com/andymccurdy/redis-py>redis 3.4.1</a><br>
- <a href=https://github.com/psf/requests>requests 2.22.0</a>

## 📲 Установка
1 - Скачивание бота 💾
  ```bash
  git clone https://github.com/Conradk10/telegram-multibot
  cd telegram-multibot/
  ```

2 - Получение API ID и ключа 🔐
  - Для начала нужно перейти по <a href="https://my.telegram.org/apps">этой</a> или <a href=https://my.telegram.org/auth>этой</a> ссылке
  - Ввести номер телефона и нажать `API development tools`
  - Скопировать `App api_id` и `App api_hash`

3 - Подготовка юзербота 🔧
  - В файл config.ini вставить `api_id` и `api_hash`
  ```bash
  nano config.ini
  ```




***ВНИМАНИЕ: Если вы будете использовать API_KEY чужого аккаунта, то ВАШ аккаунт будет удален Телеграмом!***

4 - Подготовка базы данных 📦

### Linux:
```bash
*** База данных ***
# Для Debian
sudo apt install redis-server
# Для Arch
sudo pacman -S redis-server
# Для Fedora
sudo dnf -y install redis

# Включить и запустить базу данных
service redis-server enable
service redis-server start

*** Подготовка к запуску и сам запуск ***
# Установка библиотек
pip3 install -r requirements.txt
# Запуск бота
python3 bot.py
```

### Mac OS:
```bash
*** База данных ***
# Обновление brew
brew update
# Установка БД
brew install redis
# Запуск БД
brew services start redis

*** Подготовка к запуску и запуск ***
# Установка библиотек
pip3 install -r requirements.txt
# Запуск бота
python3 bot.py
```


## 📜 Список команд
- `!about` - о проекте
- `!action` - вкл/выкл чат действие
- `!setaction {action}` - установить чат действие {action}
- `!actionlist` - список доступных чат действий
- `!autodel` - вкл/выкл автоудаление сообщений
- `!autodel {time}` - изменить время {time} автоудаления сообщений в секундах
- `!ban` - заблокировать юзера (через ответ)
- `!unban` - разблокировать юзера (через ответ)
- `!setcmd {cmd}` - установить быструю команду {cmd} на вложение (через ответ)
- `!cmdlist` - список доступных быстрых команд
- `!delcmd {cmd}` - удалить быструю команду {cmd}
- `!now` - текущие дата и время
- `!addf {text}` - добавить фразу {text} в список фраз (Spam)
- `!delf {text}` - удалить фразу {text} из сипска фраз (Spam)
- `!listf` - отобразить список доступных фраз (Spam)
- `!clearf` - оичстить список доступных фраз (Spam)
- `!pin` - закрепить сообщение (через ответ)
- `!unpin` - открепить сообщение (через ответ)
- `!kick` - кикнуть юзера (через ответ)
- `!help` - отобразить все доступные команды
- `!userid` - узнать id юзера (через ответ)
- `!nobody` - выключить отображение последнего времени онлайна
- `!everybody` - включить отображение последнего времени онлайна
- `!mark` - добавить/удалить чат в список отмеченных чатов
- `!marklist` - отобразить список отмеченных чатов
- `!mute` - заглушить (через ответ)
- `!offline` - вкл/выкл режим не беспокоить (когда не в сети)
- `!plugins` - отобразить список плагинов и команд к ним
- `!server` - отобразить системный монитор сервера
- `!settings` - отобразить настройки бота
- `!spam {n}` - спам пересылкой {n} количество раз (через ответ)
- `!spamf {n}` - спам {n} раз фразами
- `!connect` - установить соединение по ssh с сервером
- `!disconnect` - разорвать соединение по ssh с сервером

## 📝 Планы на будущее
 - Оптимизировать код
 - Добавить больше плагинов (каких? пока секрет)
 - Добавить плагин: отсчет до указанной пользователем даты, уведомление о наступившей дате
 - Список будет дополняться...
