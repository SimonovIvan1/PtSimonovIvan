
<p align="center">Министерство науки и высшего образования Российской Федерации</p>
<p align="center">Федеральное государственное бюджетное образовательное учреждение</p>
<p align="center">высшего образования</p>
<p align="center">«Рязанский государственный радиотехнический университет имени В.Ф.Уткина»</p>
<br>
<br>
<p align="center">Дисциплина: Технология программирования</p>
<p align="center">Анализ предметной области</p>
<br>
<br>
<br>
<p align="right">Выполнил: ст. гр.1315 Симонов И.Ю.</p>
<p align="right">Проверил: ст. пр. Аникеев Д.В.</p>
<br>
<br>
<br>
<br>
<p align="center">Рязань 2022г.</p>
<hr>
<br>
<h2 align="center">Введение</h2>

<p>  В сфере продажи стройматериалов главными задачами является обеспечить быструю и автоматизированную работу персонала. В данной сфере это особенно важно, что обуславливает широкое применение пакетов и программ, благодаря которым повышается скорость обработки заказов и дальнейшая их транспортировка клиенту. <br>
Цель работы: выявить проблемные вопросы и поставить задачи по их устранению.

</p>

<br>
<h2 align="center">1. Предметная область</h2>
<h3 align="center">1.1 Исследование предметной области</h3>
<span>  
  В обязанности магазина стройматериалов входит продажа строительных материалов.<br> 
  Компания представляет собой предприятие, в котором ведётся учёт материала на складе, учет полученной прибыли, и многое другое. БД содержат в себе информацию о строительных материалах, поставщиках, покупателях. В случае заказа того или иного материала, данные о клиенте будут браться из базы данных. То есть для покупки строительных материалов, понадобится заполнить бланк заказов и внести в неё свои данные. После этого по номеру заказа можно будет получить квитанцию на оплату заказанных услуг (в данном случае товара). Приобретённый материал заноситься в базу данных, также, как и информация о том, какая его цена, дата покупки, общая стоимость доставки, а также информацию о покупателе.<br>
  Выходная информация представлена выходными отчетами. Отчеты обладают финансовыми данными (цена товара, общая стоимость поставок, суммы заказов). Отчет «Заказчики» содержит информацию обо всех заказчиках компании. Состоит из: уникального номера заказчика, ФИО заказчика, номера телефона, адреса
  Отчет «Поставки» содержит информацию о поставках товара за отчетный год. Состоит из информации о поставщике, товаре, количестве, дате, а также предоставляет информацию о расходах по месяцам и за отчетный год. <br>
  Отчет «Заказы» предоставляет информацию о заказах сгруппированным по заказчикам и предоставляющий информацию о ФИО заказчика, наименовании товара, его количестве и о дате заказа<br>
  Входным оперативно-учетным документом является накладная о заказах. Она предназначена для определения стоимости, адреса доставки и другой информации доставляемого товара. Составляется при каждом новом заказе.

</span>

<h3 align="center">1.2 Описание и создание BPMN-диаграммы</h2>
<span> Точкой входа служит получение заказа от покупателя. Менеджер по продажам оформляет его и отправляет информацию сборщику товаров, который проверяет наличие товаров на складе. </br>
Если весь товар имеется в наличии, то сборщик собирает заказ и передаёт информацию о статусе сборки заказа и сроках поставки менеджеру по продажам.</br>
Если товаров в наличии нет, то сборщик передаёт информацию менеджеру по продажам. Менеджер выполняет запрос в отдел закупки. Информация о заказе переходит в отдел закупки к другому исполнителю – менеджеру по закупкам, что наглядно видно на схеме, и уже этот исполнитель создает заказ поставщику. После ответа о сроках поставки, менеджер по закупкам передаёт эту информацию менеджеру по продажам.</br>
После получения информации о сроках поставки, менеджер по продажам сообщает их клиенту и уточняет, удобно ли клиенту ожидать.</br>
Если сроки доставки устроили клиента, предлагаем на выбор 2 способа оплаты: наличный расчёт и безналичный. После успешного получения заказа, клиент оплачивает доставку. </br>
В случае если клиент не согласен на сроки доставки, отменяем заказ. 
</span>

<h3 align="center">BPMN-диаграмма</h3>

![alt text](https://github.com/SimonovIvan1/PtSimonovIvan/blob/main/BPMN.png?raw=true)

<h3 align="center">1.3 Проблематика предметной области</h3>
<span>Основные трудности при реализации проекта связаны с большой загруженностью менеджера по продажам и сборщика, из-за чего снижается эффективность работы магазина.</span>  

