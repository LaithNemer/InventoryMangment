<h2>Inventory mangment system</h2>
This project is an inventory management system designed to optimize inventory tracking and management processes.
<br> the picture is describe the ER digram:

![Capture](https://github.com/LaithNemer/InventoryMangment/assets/130616174/681b838f-b404-48d1-b233-6449dea7f5eb)
<br>every entity in the system must do all oparition which can see this notes in the file :
[Inventory mangment (1).pdf](https://github.com/LaithNemer/InventoryMangment/files/14893880/Inventory.mangment.1.pdf)
<br>
using swaager editor i designed system :
[swagger editor](https://app.swaggerhub.com/apis/ISLEIMEYYEHLITH/1InventoryManagement/1.0.0-oas3.1)

<br>



<h3>how it work : </h3>
i will use spring boot as framework on java language 
and i will use mvc design pattern where do 4 packges (controller,entity,service,and repositry).<br>
first must insert data in customer (name of customer) after that can insert order for the customer <br>
and must insert information about supplier until you are able to enter data on item 
when finched insert data for any entity can do all oparitions from post,put,delete,and get.

<h3>Description for every packge</h3>
<h4>Entity : </h4>
1.customer:have name and id  as a attrubite <br>
2.order :have cuurent date ,total price ,id and customer id which is forenkey on customer<br>
3.Inventory: have id and quantity as a attrubite <br>
4.Item: have id,price,name, expirationdate ,inventoryid which is forenkey on inventory and 
orderId which is forenkey on order<br>

<h4>Controller : </h4>
1.customer controller : which can manage all oparition from delete,put,post,update inside this class <br>
2.order controller : which can manage all oparition from delete,put,post,update inside this class <br>
3.Inventory Controller: which can manage all oparition from delete,put,post,update inside this class <br>
4.Item controller: which can manage all oparition from delete,put,post,update inside this class <br>


<h4>Service : </h4>
1.customer service : using this class can do the oparitions <br>
2.order service :using this class can do the oparitions <br>
3.inventory service:using this class can do the oparitions <br>
4.item service :using this class can do the oparitions <br>

<h4>Repositry : They are an interferesis  </h4>
1.customer repositry <br>
2.order repositry<br>
3.item repositry<br>
4.inventory repositry<br>


<h4>Example on insert data </h4>
1.customer :
{
  "id": 1,
  "name": "laith nemer"
}<br>
2.Inventory<br>
{
  "id": 2,
  "quantity": 220
}
<br>

3.order : <br>
{
  "id": 2,
  "currentdate": "2024-04-07",
  "totalprice": 300,
  "customer": {
    "id": 1,
  }
}

<br>
4.Item : <br>

{
  "itemid": 2,
  "price": 221,
  "name": "chips",
  "expirationdate": "2024-04-07",
  "inventory": {
    "id": 2,
    "quantity": 0
  },
  "order": {
    "id": 2,
   
    
  }
}











