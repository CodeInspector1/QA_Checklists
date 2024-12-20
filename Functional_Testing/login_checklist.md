# Чек-лист для тестирования страницы входа

## 1. Позитивные сценарии
- [ ] При вводе **корректного логина и пароля** пользователь успешно выполняет вход в систему.  
- [ ] Кнопка **"Войти"** активируется после заполнения всех обязательных полей.  
- [ ] Пользователь перенаправляется на **главную страницу** или **личный кабинет** после успешного входа.   
- [ ] Проверка **кросс-браузерности**: успешный вход в браузерах (Chrome, Firefox, Safari, Edge).  
- [ ] Время ответа сервера после ввода данных не превышает допустимый порог (например, < 2 секунд).  

---

## 2. Негативные сценарии
- [ ] При вводе **некорректного логина или пароля** выводится сообщение "Неправильный логин или пароль".  
- [ ] Поля **логин и пароль** не принимают пустые значения, отображается подсказка "Это обязательное поле".  
- [ ] Несколько неудачных попыток входа блокируют пользователя (если предусмотрена функция блокировки).    
- [ ] При вводе **пустых пробелов** в полях логина/пароля выводится сообщение об ошибке.  
- [ ] Поле логина не принимает **некорректные символы** (например, `#,$,%,&`).    

---

## 3. Проверка валидации полей
- [ ] Поле логина принимает только корректный **email** (например, `test@test.com`).  
- [ ] В случае неверного формата email отображается сообщение: "Введите корректный email".  
- [ ] Поле пароля проверяет минимальное количество символов (например, **не менее 8 символов**).  
- [ ] Проверка максимальной длины пароля (например, **не более 20 символов**).  
- [ ] Поле пароля принимает только **допустимые символы**: латинские буквы, цифры и специальные символы.  

---

## 4. Проверка UI/UX
- [ ] Поля ввода логина и пароля соответствуют дизайну (цвет рамок, размеры, шрифты).  
- [ ] Кнопка **"Войти"** неактивна при незаполненных обязательных полях.  
- [ ] Кнопка **"Войти"** визуально меняет цвет или стиль при наведении.  
- [ ] Сообщения об ошибках (валидация, неверные данные) читаемы и понятны пользователю.  
- [ ] Плейсхолдеры в полях логина и пароля отображают правильный текст ("Введите логин", "Введите пароль").  
- [ ] Текст на кнопках и в сообщениях соответствует требованиям локализации (если доступно несколько языков).  
- [ ] Логотип и основные элементы страницы отображаются корректно и не перекрываются.   

---

## 5. Граничные значения (Boundary Testing)
- [ ] Ввод логина длиной **минимально допустимое количество символов** (например, 1 символ).  
- [ ] Ввод логина с **максимальной длиной** (например, 255 символов).  
- [ ] Ввод пароля длиной **минимально допустимое количество символов** (например, 8 символов).  
- [ ] Ввод пароля с **максимальной длиной** (например, 20 символов).  

---

## 6. Кросс-браузерное и кросс-платформенное тестирование
- [ ] Проверка корректности отображения страницы входа в различных браузерах:  
  - Chrome  
  - Firefox  
  - Safari  
  - Edge  
- [ ] Тестирование на мобильных устройствах (Android/iOS).  
- [ ] Проверка работы на различных разрешениях экрана (адаптивный дизайн).  

---

## 7. Проверка на восстановление пароля
- [ ] Ссылка **"Забыли пароль?"** присутствует и кликабельна.  
- [ ] При нажатии на ссылку открывается страница для восстановления пароля.  
- [ ] Ввод корректного email отправляет письмо для восстановления пароля.  
- [ ] Сообщение о неправильном email отображается корректно.  

---
