# uftocp

1. Включить модуль
2. Настроить нужные поля в admin/commerce/config/checkout/form/pane/account
3. Изменить rules "Создание новой учётной записи для анонимного заказа", добавив для полей такой код
<?php
echo $commerce_order->data['field_phone'][0]['value'];
?>

Для полей с несколькими значениями можно устанавливать данные через action "выполнить php"