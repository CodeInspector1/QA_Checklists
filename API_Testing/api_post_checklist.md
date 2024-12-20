# Чек-лист для тестирования POST-запросов

## Позитивные сценарии
- [ ] **Статус-код ответа** `201 Created` при успешном создании ресурса.  
- [ ] **Тело ответа** содержит ID нового ресурса.  
- [ ] **В базе данных** создаётся запись с переданными значениями.  
- [ ] **Поля соответствуют типам данных** и ограничениям (например, длина строк).  
- [ ] **Ответ возвращается в корректном формате**.

## Негативные сценарии
- [ ] **Ошибка 400 Bad Request**, если отсутствуют обязательные поля в теле запроса.  
- [ ] **Ошибка 422 Unprocessable Entity**, если переданы некорректные данные (например, email в неверном формате).  
- [ ] **Статус 401 Unauthorized** при отсутствии или неверном токене.  
- [ ] **Ошибка 409 Conflict** при создании дублирующегося ресурса.
