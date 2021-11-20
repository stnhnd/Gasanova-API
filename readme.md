# Навигация
+ [Товары](#Товары)
+ [Категории](#Категории)
+ [Цвета](#Цвета)
+ [Размеры](#Размеры)
+ [Коллекции](#Коллекции)
+ [Заказы](#Заказы)
+ [Брошенные корзины](#брошенные-корзины)
+ [Остатки товаров](#остатки-товаров)

# Товары
__[Наверх ↑](#Навигация)__

<br>

**Получить все товары**

> GET Запрос
```
/api/get-products
```

> Ответ
``` json
[
    {
        "category": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9",
        "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
        "priceUAH": 15000,
        "priceUSD": 15000,
        "priceRUB": 15000,
        "newPriceUAH": 14000,
        "newPriceUSD": 12000,
        "newPriceRUB": 0,
        "titleUK": "test",
        "titleRU": "test",
        "titleEN": "test test",
        "link": "test-test",
        "article": "test",
        "season": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            },
            {
                "color": "53d38295-c425-4f01-8111-74338b71f92a",
                "sizes": [
                    {
                        "amount": 5,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    },
                    {
                        "amount": 8,
                        "size": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b"
                    }
                ]
            }
        ],
        "frontImage": "front.jpg",
        "backImage": "back.jpg",
        "photos": [
            "photo-1.jpg",
            "photo-2.jpg",
            "photo-3.jpg",
            "photo-4.jpg"
        ],
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test"
    },
    {
        "category": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9",
        "uuid": "826fe6ff-b5e9-4fe7-8bd2-5227586532ac",
        "priceUAH": 18000,
        "priceUSD": 32000,
        "priceRUB": 21000,
        "newPriceUAH": 0,
        "newPriceUSD": 0,
        "newPriceRUB": 0,
        "titleUK": "test",
        "titleRU": "test",
        "titleEN": "test test",
        "link": "test1",
        "article": "test",
        "season": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 0,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            }
        ],
        "frontImage": "front.jpg",
        "backImage": "back.jpg",
        "photos": [
            "photo-1.jpg",
            "photo-2.jpg",
            "photo-3.jpg",
            "photo-4.jpg"
        ],
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test"
    }
]
```

<br>

**Добавить\Редактировать товар**

> POST Запрос
```
/api/product
```

> Body

``` json
{
    "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
    "titleUK": "test",
    "titleRU": "test",
    "titleEN": "test test",
    "article": "test",
    "category": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9",
    "season": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87",
    "params": [
        { 
        "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9", 
        "sizes": [{ "size": "6da37ab4-ac0c-4668-b161-71e8d128c287", "amount": 10 }] 
        },
        { 
        "color": "53d38295-c425-4f01-8111-74338b71f92a", 
        "sizes": [
            { "size": "6da37ab4-ac0c-4668-b161-71e8d128c287", "amount": 5 },
            { "size": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b", "amount": 8 }
            ] 
        }
        ],
    "priceUAH": 15000,
    "priceRUB": 15000,
    "priceUSD": 15000,
    "newPriceUAH": 14000,
    "newPriceRUB": 0,
    "newPriceUSD": 12000,
    "frontImage": "front.jpg",
    "backImage": "back.jpg",
    "photos": [
      "photo-1.jpg",
      "photo-2.jpg",
      "photo-3.jpg",
      "photo-4.jpg"
    ],
    "aboutRU": "test",
    "aboutEN": "test",
    "aboutUK": "test",
    "compoRU": "test",
    "compoEN": "test",
    "compoUK": "test"
}

```

<br>

**Удалить товар**

> POST Запрос
```
/api/delete
```

> Body

``` json
{
    "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915"
}
```

<br>

# Категори
__[Наверх ↑](#Навигация)__
<br>

**Получить все категории**

> GET Запрос
```
/api/get-categories
```

> Ответ
``` json
[
    {
        "uuid": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9",
        "titleRU": "платья",
        "titleEN": "dresses",
        "titleUK": "сукні",
        "imageURL": "gallery/1625321873748-dress.png"
    }
]
```

<br>

**Добавить\Редактировать категорию**

> POST Запрос
```
/api/category
```

> Body
``` json
{
    "uuid": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9",
    "titleRU": "платья",
    "titleEN": "dresses",
    "titleUK": "сукні",
    "imageURL": "gallery/1625321873748-dress.png"
}
```

<br>

**Удалить категорию**

> POST Запрос
```
/api/delete-category
```

> Body

``` json
{
    "uuid": "0273b74e-9a3c-4392-bfeb-b427a47d9cb9"
}
```

<br>

# Цвета
__[Наверх ↑](#Навигация)__
<br>

**Получить все цвета**

> GET Запрос
```
/api/get-colors
```

> Ответ
``` json
[
    {
        "uuid": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
        "hex": "#FFFFFF"
    },
    {
        "uuid": "53d38295-c425-4f01-8111-74338b71f92a",
        "hex": "#E5B936"
    }
]
```

<br>


**Добавить\Редактировать цвет**

> POST Запрос
```
/api/colors
```

> Body

``` json
{
    "uuid": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
    "title": "M"
}
```

<br>

**Удалить цвет**

> POST Запрос
```
/api/delete-color
```

> Body

``` json
{
    "uuid": "4347da5d-4da2-4074-9136-a6d86a2f7ed9"
}
```

<br>

# Размеры
__[Наверх ↑](#Навигация)__
<br>

**Получить все размеры**

> GET Запрос
```
/api/get-sizes
```

> Ответ
``` json
[
    {
        "uuid": "6da37ab4-ac0c-4668-b161-71e8d128c287",
        "title": "S"
    },
    {
        "uuid": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b",
        "title": "M"
    }
]
```

<br>

**Добавить\Редактировать размер**

> POST Запрос
```
/api/size
```

> Body
``` json
{
    "uuid": "6da37ab4-ac0c-4668-b161-71e8d128c287",
    "title": "S"
}
```

<br>

**Удалить размер**

> POST Запрос
```
/api/delete-size
```

> Body

``` json
{
    "uuid": "6da37ab4-ac0c-4668-b161-71e8d128c287"
}
```

<br>

# Коллекции
__[Наверх ↑](#Навигация)__
<br>

**Получить все коллекции**

> GET Запрос
```
/api/get-seasons
```

> Ответ
``` json
[
    {
        "uuid": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87",
        "title": "SS'17"
    }
]
```

<br>

**Добавить\Редактировать коллекцию**

> POST Запрос
```
/api/season
```

> Body
``` json
{
    "uuid": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87",
    "title": "SS'17"
}
```

<br>

**Удалить коллекцию**

> POST Запрос
```
/api/delete-season
```

> Body

``` json
{
    "uuid": "7e5d6ded-d86b-4787-9ee7-0d4392aa0b87"
}
```

<br>

# Заказы
__[Наверх ↑](#Навигация)__
<br>

**Получить все заказы**

> GET Запрос
```
/api/get-orders
```

> Ответ
``` json
[
    {
        "uuid": "b69ea756-a706-4583-9adb-08892c93840c",
        "status": "new",
        "orderId": "454744237",
        "date": "10/20/2021",
        "time": "18:05",
        "firstname": "Максим",
        "lastname": "Калашник",
        "email": "minimalwbd@gmail.com",
        "phone": "+380123123122",
        "comment": "",
        "delivery": "DHL",
        "deliveryStatus" "formed"
        "city": "",
        "department": "",
        "address": "test",
        "total": "42000",
        "currency": "uah",
        "cart": [
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 1,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                        "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9"
                    }
                ]
            },
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 1,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                        "color": "53d38295-c425-4f01-8111-74338b71f92a"
                    }
                ]
            },
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 1,
                        "size": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b",
                        "color": "53d38295-c425-4f01-8111-74338b71f92a"
                    }
                ]
            }
        ]
    },
    {
        "uuid": "41a6cd30-7111-4126-87ce-12c1e6399cc5",
        "status": "new",
        "orderId": "454754817",
        "date": "10/20/2021",
        "time": "18:39",
        "firstname": "Максим",
        "lastname": "Калашник",
        "email": "minimalwbd@gmail.com",
        "phone": "+380123123122",
        "comment": "",
        "delivery": "DHL",
        "deliveryStatus" "formed"
        "city": "",
        "department": "",
        "address": "test",
        "total": "70000",
        "currency": "uah",
        "cart": [
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 1,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                        "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9"
                    }
                ]
            },
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 1,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                        "color": "53d38295-c425-4f01-8111-74338b71f92a"
                    }
                ]
            },
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": 3,
                        "size": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b",
                        "color": "53d38295-c425-4f01-8111-74338b71f92a"
                    }
                ]
            }
        ]
    }
]
```

<br>

**Обновить заказ**

> POST Запрос
```
/api/update-order
```

> Body
``` json
{   
    "uuid": "c70ce075-6eb3-4035-b8ad-6bbb7866fc77",
    "status": "new || success || not-paid",
    "ttn": "ttn number",
    "deliveryStatus": "formed || sent",
    "comment": "test",
    "cart": [
        {
            "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
            "params": [
                {
                    "count": "1",
                    "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                    "color": "53d38295-c425-4f01-8111-74338b71f92a"
                }
            ]
        },
        {
            "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
            "params": [
                {
                    "count": "1",
                    "size": "fdf5ba52-838f-41b2-8eeb-99740f11cf6b",
                    "color": "53d38295-c425-4f01-8111-74338b71f92a"
                }
            ]
        }
    ]
}
```

<br>

# Брошенные корзины
__[Наверх ↑](#Навигация)__
<br>

**Получить все брошенные корзины**

> GET Запрос
```
/api/get-abandoned
```

> Body
``` json
[
    {
        "firstname": "test",
        "lastname": "test",
        "phone": "+38012 312 3123",
        "email": "minimalwbd@gmail.com",
        "comment": "test",
        "cart": [
            {
                "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
                "params": [
                    {
                        "count": "1",
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287",
                        "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9"
                    }
                ]
            }
        ]
    }
]
```

# Остатки товаров
__[Наверх ↑](#Навигация)__
<br>

**Получить остатки**

> GET Запрос
```
/api/get-sku
```

> Body
``` json
[
    {
        "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            }
        ]
    },
    {
        "uuid": "826fe6ff-b5e9-4fe7-8bd2-5227586532ac",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 15,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            }
        ]
    }
]
```

<br>

**Обновить остатки**

> POST Запрос
```
/api/update-sku
```

> Body
``` json
[
    {
        "uuid": "e33cc2b5-f593-447b-b47c-ee6fa448e915",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            }
        ]
    },
    {
        "uuid": "826fe6ff-b5e9-4fe7-8bd2-5227586532ac",
        "params": [
            {
                "color": "4347da5d-4da2-4074-9136-a6d86a2f7ed9",
                "sizes": [
                    {
                        "amount": 15,
                        "size": "6da37ab4-ac0c-4668-b161-71e8d128c287"
                    }
                ]
            }
        ]
    }
]
```
