# GetCID API для русского сайта и пользователей/Разработчики
GetCID API и PIDMS License Checker API - автоматизируйте активацию продуктов Microsoft и проверку лицензий с помощью простого API.

**GetCID API и PIDMS License Checker API Документация**

Добро пожаловать в документацию по API GetCID и PIDMS License Checker! Этот гид содержит подробную информацию о том, как интегрировать наши API для активации продуктов Microsoft и проверки лицензий. Если вы хотите просто получить CID, перейдите по ссылке: **[GetCID Services](https://msconfirmationid.com/getcid-api/)**.

🌟 **Обзор**  
GetCID и PIDMS License Checker — это сервисы для активации и проверки продуктов Microsoft.  
Наши API предоставляют разработчикам инструменты для автоматизации этих процессов:  
- **GetCID API**: автоматическая генерация кодов подтверждения (CID) для активации продуктов Microsoft.  
- **PIDMS License Checker API**: проверка лицензионных ключей Microsoft на подлинность и соответствие.  

Больше информации доступно на странице **[API Services](https://msconfirmationid.com/getcid-api/)**.

🚀 **Как начать**  
Для начала работы с нашими API выполните следующие шаги:  
1. **Регистрация**: получите API-ключ на странице [API Services](https://msconfirmationid.com/getcid-api/).  
2. **Документация**: ознакомьтесь с конечными точками и параметрами API.  
3. **Интеграция**: внедрите API в свои приложения с использованием предоставленных примеров кода.  

🔑 **Аутентификация**  
Все запросы к API требуют наличия API-ключа. Укажите ключ в заголовке запроса следующим образом:  
`Authorization: Bearer YOUR_API_KEY`

📘 **Конечные точки API**  

1. **GetCID API**  
   - **Endpoint**: `/api/getcid`  
   - **Метод**: POST  
   - **Описание**: Генерация кода подтверждения (CID) для активации продуктов Microsoft.  

   **Параметры запроса**:  
   - `installation_id` (string): Идентификатор установки Microsoft.  
   - `product_id` (string): Идентификатор продукта Microsoft.  

   **Пример запроса**:  
   ```json
   POST /api/getcid
   Authorization: Bearer YOUR_API_KEY
   Content-Type: application/json

   {
     "installation_id": "123456789012345678901234567890123456789012345678901234567",
     "product_id": "XXXXX-XXXXX-XXXXX-XXXXX"
   }
   ```  

   **Пример ответа**:  
   ```json
   {
     "confirmation_id": "123456789012345678901234567"
   }
   ```

2. **PIDMS License Checker API**  
   - **Endpoint**: `/api/license-check`  
   - **Метод**: POST  
   - **Описание**: Проверка лицензионного ключа Microsoft.  

   **Параметры запроса**:  
   - `license_key` (string): Лицензионный ключ Microsoft.  

   **Пример запроса**:  
   ```json
   POST /api/license-check
   Authorization: Bearer YOUR_API_KEY
   Content-Type: application/json

   {
     "license_key": "XXXXX-XXXXX-XXXXX-XXXXX-XXXXX"
   }
   ```  

   **Пример ответа**:  
   ```json
   {
     "valid": true,
     "product": "Microsoft Office 2021 Professional Plus",
     "expiration_date": "2025-12-31"
   }
   ```

💻 **Советы по интеграции**  
- Храните API-ключ в безопасности, не размещайте его в клиентском коде.  
- Обрабатывайте ответы API, включая ошибки.  
- Следите за использованием API, чтобы не превышать лимиты запросов.  

🛠️ **Поддержка и контакты**  
Если у вас возникли вопросы или вам нужна помощь, свяжитесь с нами:  
- **Telegram**: [@CIDAdmin](https://t.me/CIDAdmin)  
- **Email**: [care@msconfirmationid.com](mailto:care@msconfirmationid.com)  
- **Skype**: live:.cid.afc21522bf98cf1b  
- **Website**: [GetCID Services](https://msconfirmationid.com/getcid-api/)  

Спасибо за выбор наших сервисов! 🚀
**Примечание:** Оплата в RUB и криптовалюте. Для помощи: Telegram: [@CIDAdmin](https://t.me/CIDAdmin), Email: [care@msconfirmationid.com](mailto:care@msconfirmationid.com), Skype: live:.cid.afc21522bf98cf1b.
