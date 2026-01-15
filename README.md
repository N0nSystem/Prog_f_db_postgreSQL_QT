<h3>Подключение к локальному серверу с БД postgreSQL:</h3> <br>
<b>ip</b> - 192.168.0.150<br>
<b>port</b> - 5432<br>
Бд имеет таблицы:<br>
<ul>
  <li>client</li>
  <li>orders</li>
</ul>
<h5>client:</h5>
<ol>
  <li>id</li>
  <li>full_name</li>
  <li>phone</li>
  <li>email</li>
</ol>
<h5>orders:</h5>
<ol>
  <li>id</li>
  <li>client_id</li>
  <li>shipment_date</li>
  <li>contract_number</li>
  <li>quantity</li>
</ol>
 <h3>Программа выполняет SQL запросы,<br>
 такие как:</h3>
 <ul>
  <li><b><i>SELECT * FROM client ORDER BY id</i></b> - запросить у бд список клиентов и отсортировать по id</li>
  <li><b><i>"INSERT INTO client (full_name, phone, email) " <br>
    "VALUES ('%1', '%2', '%3')"</i></b> - создать нового клиента используя данные,которые вводит пользователь</li>
  
</ul>


 <h2><b>ВНИМАНИЕ:</b></h2> <h4><b>Программа не запустится если нет сервера</b></h4>
