# Инструкция по загрузке на GitHub и настройке GitHub Pages

## Шаг 1: Создание репозитория на GitHub

1. Перейдите на [GitHub.com](https://github.com) и войдите в свой аккаунт
2. Нажмите кнопку **"+"** в правом верхнем углу и выберите **"New repository"**
3. Заполните форму:
   - **Repository name**: `Practicum-2` (или любое другое имя)
   - **Description**: "Концепция сервиса коммуникации жителей и органов местного самоуправления"
   - Выберите **Public** (публичный репозиторий)
   - **НЕ** ставьте галочки на "Initialize this repository with a README" (у нас уже есть файлы)
4. Нажмите **"Create repository"**

## Шаг 2: Подключение локального репозитория к GitHub

После создания репозитория GitHub покажет вам инструкции. Выполните следующие команды в терминале (замените `YOUR_USERNAME` на ваш GitHub username):

```powershell
git remote add origin https://github.com/YOUR_USERNAME/Practicum-2.git
git branch -M main
git push -u origin main
```

Если у вас еще не настроена аутентификация, GitHub может попросить вас войти. Используйте Personal Access Token вместо пароля.

## Шаг 3: Настройка GitHub Pages

1. Перейдите в ваш репозиторий на GitHub
2. Нажмите на вкладку **"Settings"** (в верхнем меню репозитория)
3. В левом меню найдите раздел **"Pages"** (в секции "Code and automation")
4. В разделе **"Source"** выберите:
   - Branch: `main`
   - Folder: `/ (root)`
5. Нажмите **"Save"**

## Шаг 4: Доступ к вашему сайту

Через несколько минут ваш сайт будет доступен по адресу:
```
https://YOUR_USERNAME.github.io/Practicum-2/
```

GitHub автоматически обновит сайт при каждом новом коммите в ветке `main`.

## Полезные команды Git

### Добавить изменения и отправить на GitHub:
```powershell
git add .
git commit -m "Описание изменений"
git push
```

### Проверить статус репозитория:
```powershell
git status
```

### Посмотреть историю коммитов:
```powershell
git log
```

## Примечания

- Убедитесь, что файл `index.html` находится в корне репозитория (это главная страница)
- GitHub Pages автоматически использует `index.html` как главную страницу
- Изменения на сайте появятся через 1-2 минуты после push

