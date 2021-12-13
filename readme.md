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
        "titleRU": "test",
        "titleEN": "test test",
        "titleUK": "test",
        "_id": "61a4afc2c63be8e71aeb81b8",
        "link": "test-test",
        "article": "test",
        "category": "61a3ade5a9d75713f47d022f",
        "season": "61a3ba49c9a4394f26faf593",
        "params": [
            {
                "color": {
                    "photos": [
                        "photo-1.jpg",
                        "photo-2.jpg",
                        "photo-3.jpg",
                        "photo-4.jpg"
                    ],
                    "_id": "61a3b9f3f5015805829cd79e",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": {
                    "photos": [],
                    "_id": "61a3b9f3f5015805829cd795",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            }
        ],
        "priceUAH": 15000,
        "priceUSD": 15000,
        "priceRUB": 15000,
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test",
        "__v": 0
    }
]
```

<br>

**Добавить\Обновить\Удалить товары**

> POST Запрос
```
/api/products
```

> Body

``` json
[
    {
        "priceUAH": 15000,
        "priceUSD": 15000,
        "priceRUB": 15000,
        "newPriceUAH": 0,
        "newPriceUSD": 0,
        "newPriceRUB": 0,
        "_id": "61a4afc2c63be8e71aeb81b8",
        "titleUK": "test",
        "titleRU": "test",
        "titleEN": "test test",
        "link": "test-test",
        "article": "test",
        "category": "61a3ade5a9d75713f47d022f",
        "season": "61a3ba49c9a4394f26faf593",
        "params": [
            {
                "color": {
                    "_id": "61a3b9f3f5015805829cd79e",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg",
                    "photos": [
                        "photo-1.jpg",
                        "photo-2.jpg",
                        "photo-3.jpg",
                        "photo-4.jpg"
                    ]
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": {
                    "_id": "61a3b9f3f5015805829cd795",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            }
        ],
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test",
        "__v": 0
    }
]

```

<br>

# Категории
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
        "_id": "61a3ade5a9d75713f47d022f",
        "titleRU": "платья",
        "titleEN": "dresses",
        "titleUK": "сукні",
        "imageURL": "dress.png",
    }
]
```

<br>

**Добавить\Редактировать\Удалить категории**

> POST Запрос
```
/api/categories
```

> Body
``` json
[
    {
        "_id": "61a3ade5a9d75713f47d022f",
        "titleRU": "платья",
        "titleEN": "dresses",
        "titleUK": "сукні",
        "imageURL": "dress.png"
    }
]
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
        "hex2": "#FF6C37",
        "pattern": "chameleon",
        "_id": "61a3b9f3f5015805829cd795",
        "hex1": "#FFFFFF",
        "__v": 0
    },
    {
        "hex2": "#FF69B4",
        "pattern": "",
        "_id": "61a3b9f3f5015805829cd79e",
        "hex1": "#FFFFFF",
        "__v": 0
    }
]
```

<br>


**Добавить\Редактировать\Удалить цвета**

> POST Запрос
```
/api/colors
```

> Body

``` json
[
    {
    "_id": "61a3b9f3f5015805829cd795",
    "hex1": "#FFFFFF",
    "hex2": "#FF6C37",
    "pattern": "chameleon"
    },
    {
    "_id": "61a3b9f3f5015805829cd79e",
    "hex1": "#FFFFFF",
    "hex2": "#FF69B4",
    "pattern": ""
    }
]
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
        "_id": "61a3ba2e730503f53b36e63f",
        "title": "M",
    },
    {
        "_id": "61a3ba49c9a4394f26faf591",
        "title": "S",
    }
]
```

<br>

**Добавить\Редактировать\Удалить размеры**

> POST Запрос
```
/api/sizes
```

> Body
``` json
[
    {
        "_id": "61a3ba2e730503f53b36e63f",
        "title": "M"
    },
    {
        "_id": "61a3ba49c9a4394f26faf591",
        "title": "S"
    }
]
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
        "_id": "61a3ba49c9a4394f26faf593",
        "title": "SS'17"
    }
]
```

<br>

**Добавить\Редактировать\Удалить коллекцию**

> POST Запрос
```
/api/seasons
```

> Body
``` json
[
    {
        "_id": "61a3ba49c9a4394f26faf593",
        "title": "SS'17"
    }
]
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
        "status": "not-paid",
        "_id": "61b48ec73db8c614f08344f8",
        "date": "12/11/2021",
        "time": "13:43",
        "firstname": "test",
        "lastname": "test",
        "email": "minimal.wbd@gmail.com",
        "phone": "+38012 312 3123",
        "comment": "test",
        "delivery": "DHL",
        "city": "",
        "department": "",
        "address": "test",
        "total": "30000",
        "currency": "uah",
        "deliveryStatus": "formed",
        "userId": null,
        "cart": [
            {
                "params": [
                    {
                        "count": 2,
                        "size": "61a3ba49c9a4394f26faf591",
                        "color": "61a3b9f3f5015805829cd795"
                    }
                ],
                "productId": "61a4afc2c63be8e71aeb81b8",
                "price": "15000"
            }
        ],
        "__v": 0
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
    "_id": "61a7c96f29c3d72bc4a5e8d9",
    "status": "new || success || not-paid",
    "ttn": "ttn number",
    "deliveryStatus": "formed || sent",
    "comment": "test",
    "cart": [
        {
            "params": [
                {
                    "count": 2,
                    "size": "61a3ba49c9a4394f26faf591",
                    "color": "61a3b9f3f5015805829cd795"
                }
            ],
            "productId": "61a4afc2c63be8e71aeb81b8",
            "price": "15000"
        }
    ],
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
        "firstname": "Артем",
        "lastname": "Прокофьев",
        "phone": "+380 512 312 312",
        "email": "fake@gmail.com",
        "comment": "",
        "cart": {
            "items": [
                {
                    "productId": "61a4afc2c63be8e71aeb81b8",
                    "params": [
                        {
                            "count": 2,
                            "size": "61a3ba49c9a4394f26faf591",
                            "color": "61a3b9f3f5015805829cd795"
                        }
                    ]
                }
            ]
        }
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
        "_id": "61a4afc2c63be8e71aeb81b8",
        "params": [
            {
                "color": {
                    "photos": [
                        "photo-1.jpg",
                        "photo-2.jpg",
                        "photo-3.jpg",
                        "photo-4.jpg"
                    ],
                    "_id": "61a3b9f3f5015805829cd79e",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": {
                    "photos": [],
                    "_id": "61a3b9f3f5015805829cd795",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
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
        "_id": "61a4afc2c63be8e71aeb81b8",
        "params": [
            {
                "color": {
                    "photos": [
                        "photo-1.jpg",
                        "photo-2.jpg",
                        "photo-3.jpg",
                        "photo-4.jpg"
                    ],
                    "_id": "61a3b9f3f5015805829cd79e",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": {
                    "photos": [],
                    "_id": "61a3b9f3f5015805829cd795",
                    "frontImage": "front.jpg",
                    "backImage": "back.jpg"
                },
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            }
        ]
    }
]
```
