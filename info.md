**Description (Описание)**
<p>This integration allows you to connect any GPS Tracker ( compatible with <a href='https://livegpstracks.com/'>livegpstracks</a> service) to HomeAssistant (Данная интеграция позволяет подключить любой GPS трекер (совместимый с <a href='https://livegpstracks.com/'>livegpstracks</a>) к вашему HomeAssistant)</p>



**Installation (Установка):**
<p>You need to register in the livegpstracks service and connect the tracker (the site has detailed instructions for various models) to it. After that, through the toolbar on the site we create a private link for tracking. The link looks like:</p> 
<pre><code>
https://livegpstracks.com/dv_USERID.html
</code></pre>
<p>here USERID – is ID of your livegpstracks share, it will be needed to us further </p>
<p>Then install this integration</p>

<p>Регистрируемся в сервисе livegpstracks и подключаем свой трекер (на сайте есть подробные инструкции для различных моделей). После этого через панель инструментов на сайте создаем приватную ссылку для слежения. Ссылка имеет вид:</p> 
<pre><code>
https://livegpstracks.com/dv_USERID.html
</code></pre>
<p>где USERID – цифровой ID вашей шары, он пригодится нам вдальнейшем</p>
<p>После этого установите данную интеграцию</p>



**Example configuration.yaml:**

```yaml
car_location:
  username: 'your_username'
  client_id: 'your_share_id'
```



**Configuration variables:**  
  
key | description  
:--- | :---  
**username (Required)** | the username, you registered with on livegpstracks (пользователь, под которым вы регистрировались в сервисе livegpstracks)
**client_id (Required)** | the ID of your livegpstracks share (цифровой ID, который присваивается расшаренной ссылке)
**scan_interval (Option)** | update interval, default 120 sec (интервал обновления сенсора, по умолчанию 120 сек)
