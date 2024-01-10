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

Ejemplo

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

Objeto <bold id="nueva-area">NewArea</bold> </br> <sub>Propiedades:</sub>