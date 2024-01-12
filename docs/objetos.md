## Objeto <bold id="balance-general-almacenes">*getGeneralStockReport*</bold> 
</br> <sub>Propiedades:</sub>


- mainCurrency [srtring]: </br> moneda principal

---

- result [array]: </br> arreglo de objetos *BalanceStockReport*

</br>
</br>
</br>

Objeto *BalanceStockReport*
</br> <sub>Propiedades:</sub>

- areaId [number]: </br> idenificador único de áreas

---

- areaName [string]: </br> nombre del área

---

- total_cost [number]: </br> costo total

---

- total_estimated_sales [number]: </br> total estimado de ventas

---

- total_estimated_profits [number]: </br> total estimado de ganancias


Ejemplo:

```json
{
  "mainCurrency": "CUP",
  "result": [
    {
      "areaId": 1,
      "areaName": "Almacén principal (Shop)",
      "total_cost": 0,
      "total_estimated_sales": 15000,
      "total_estimated_profits": 15000
    },
    {
      "areaId": 6,
      "areaName": "Area de Prueba - Almacén (Shop)",
      "total_cost": 0,
      "total_estimated_sales": 0,
      "total_estimated_profits": 0
    },
    {
      "areaId": 9,
      "areaName": "Almacen prueba (Shop)",
      "total_cost": 0,
      "total_estimated_sales": 0,
      "total_estimated_profits": 0
    }
  ]
}
```
</br>
</br>
</br>

## Objeto <bold id="reporte-general-almacenes">*getReportStockDisponibility*</bold> 
</br> <sub>Propiedades:</sub>

- *mainCurrency* [string]: </br> moneda principal

---

- result [array]: </br> arreglo de objetos [*ReportStockDisponibility*](#reporte-almacen)

</br>

Objeto <bold id="reporte-almacen">*ReportStockDisponibility*</bold>: </br> <sub>Propiedades:</sub>

- productId [number]: </br> identificador del producto

---

- universalCode [number]: </br> código universal del producto

---

- productName [string]: </br> nombre del producto

---

- salesCategoryName [string]: </br> nombre de la categoría

---

- disponibility [number]: </br> disponibilidad del producto

---

- total_cost [number]: </br> costo total

---

- total_estimated_sales [number]: </br> total estimado de ventas

---

- total_estimated_profits [number]: </br> total estimado de ganancias

Ejemplo:

```json
{
  "mainCurrency": "CUP",
  "result": [
    {
      "productId": 4,
      "universalCode": 4,
      "productName": "Chorizo Don Carlos Gallardo y Ramirez",
      "salesCategoryName": "Sin categoría",
      "disponibility": 9,
      "total_cost": 0,
      "total_estimated_sales": 1800,
      "total_estimated_profits": 1800
    },
    {
      "productId": 1,
      "universalCode": 1,
      "productName": "Producto prueba",
      "salesCategoryName": "Sin categoría",
      "disponibility": 44,
      "total_cost": 0,
      "total_estimated_sales": 13200,
      "total_estimated_profits": 13200
    }
  ]
}
```
</br>
</br>
</br>
## Objeto <bold id="getStateInventoryPeriod">*getStateInventoryPeriod*</bold>
</br> <sub>Propiedades:</sub>

- stockProductId [number]: </br> identificador único de un producto en un almacén

---

- productId [number]: </br> identificador único de un producto

---

- name [string]: </br> nombre del producto

---

- measure [string]: </br> unidad de medida

---

- productCategory [string]: </br> nombre de la categoría de productos

---

- productCategoryId [number]: </br> identificador de la categoría a la que pertenece el producto

---

- inStock [number]: </br> cantidad del producto en almacén

---

- entry [number]: </br> description

---

- initial [number]: </br> description

---

- movements [number]: </br> description

---

- outs [number]: </br> description

---

- sales [number]: </br> description

---

- onlineSales [number]: </br> description

---

- processed [number]: </br> description

---

- waste [number]: </br> description

---

- variations [array]: </br> description

---

- enableGroup [boolean]: </br> description

---

- groupName [string]: </br> description

---

- groupConvertion [type]: </br> description

Ejemplo:

```json
{
    "stockProductId": 8,
    "productId": 5,
    "name": "Pasta de bocaditos",
    "measure": "UNIT",
    "productCategory": "Sin categoría",
    "productCategoryId": null,
    "inStock": 70,
    "entry": 0,
    "initial": 0,
    "movements": 0,
    "outs": -2,
    "sales": -282,
    "onlineSales": 0,
    "processed": 0,
    "waste": 0,
    "variations": [],
    "enableGroup": null,
    "groupName": null,
    "groupConvertion": 1
}
```

</br>
</br>
</br>
## Objeto <bold id="newProduct">*NewProduct*</bold>
</br> <sub>Propiedades:</sub>

- *name* [string]: </br> nombre del producto

---

- *price* [number]: </br> precio del producto

---

- *salesCategoryId* [number]: </br> identicador único de la categoría de ventas a la que pertenece el producto

---

- *type* [string]: </br> [tipo de producto](../glosario.md#tipos-productos)

Ejemplo:

```json
{
  "name": "Pantalón",
  "price": 350,
  "salesCategoryId": 15,
  "type": "VARIATION"
}
```

## Objeto <bold id="producto">*Product*</bold> 
</br> <sub>Propiedades:</sub>

```json
{
  "id": 1,
  "name": "Producto prueba",
  "salesCode": "00001",
  "description": null,
  "promotionalText": null,
  "type": "STOCK",
  "showForSale": true,
  "stockLimit": true,
  "qrCode": null,
  "totalQuantity": 45,
  "measure": "UNIT",
  "suggested": false,
  "onSale": false,
  "alertLimit": null,
  "isPublicVisible": true,
  "averagePreparationTime": null,
  "elaborationSteps": null,
  "averageCost": 0,
  "isAlertable": true,
  "productCategoryId": null,
  "salesCategoryId": null,
  "groupName": null,
  "groupConvertion": 1,
  "isWholesale": null,
  "minimunWholesaleAmount": 1,
  "enableGroup": null,
  "productCategory": null,
  "salesCategory": null,
  "images": [],
  "prices": [
    {
      "price": 300,
      "codeCurrency": "CUP",
      "isMain": true,
      "priceSystemId": 1
    }
  ],
  "listManufacturations": []
  },
  "variations": []
}
```
</br>
</br>
</br>
## Objeto <bold id="Area">Area</bold>
</br> <sub>Propiedades:</sub>

- *id* [number]: </br> identificador único del área

---

- *name* [string]: </br> nombre del área

---

- *code* [string]: </br> código

---

- *description* [string]: </br> descripción del área

---

- type [string]: </br> [tipo de área](glosario.md#areas)

---

- isActive [boolean]: </br> si el área está activa o no

---

- isPublicVisible [boolean]: </br> si el área está publica

---

- isMainStock [boolean]: </br> si es o no un almacén principal

---

- allowDirectlyMovements [boolean]: </br> si está permitido o no el movimiento de productos entre áreas

Ejemplo:

```json
{
  "id": 6,
  "name": "Area de Prueba - Almacén",
  "code": null,
  "description": "Área de almacén asociada a Area de Prueba",
  "type": "STOCK",
  "isActive": true,
  "isPublicVisible": false,
  "isMainStock": false,
  "allowDirectlyMovements": false,
  "productionOrderController": false,
  "images": [],
  "business": {
    "name": "Shop"
  }
}
```

</br>
</br>
</br>
## Objeto bulkEntryStockProduct
</br> <sub>Propiedades:</sub>

- products [array]: </br>

---

- stockAreaId [number]: </br> 

---

- description [string]: </br>