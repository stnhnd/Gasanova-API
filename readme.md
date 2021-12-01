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
        "priceUAH": 15000,
        "priceUSD": 15000,
        "priceRUB": 15000,
        "newPriceUAH": 14000,
        "newPriceUSD": 0,
        "newPriceRUB": 0,
        "photos": [
            "photo-1.jpg",
            "photo-2.jpg",
            "photo-3.jpg",
            "photo-4.jpg"
        ],
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
                "color": "61a3b9f3f5015805829cd79e",
                "secondColor": "61a3b9f3f5015805829cd795",
                "pattern": "goose",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 7,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": "61a3b9f3f5015805829cd795",
                "sizes": [
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            }
        ],
        "frontImage": "front.jpg",
        "backImage": "back.jpg",
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test",
        "__v": 0
    },
    {
        "priceUAH": 16000,
        "priceUSD": 15000,
        "priceRUB": 15000,
        "newPriceUAH": 0,
        "newPriceUSD": 0,
        "newPriceRUB": 0,
        "photos": [
            "photo-1.jpg",
            "photo-2.jpg",
            "photo-3.jpg",
            "photo-4.jpg"
        ],
        "_id": "61a6280b92459c044c5db748",
        "titleUK": "test",
        "titleRU": "test",
        "titleEN": "test test",
        "link": "test-test",
        "article": "test",
        "category": "61a3ade5a9d75713f47d022f",
        "season": "61a3ba49c9a4394f26faf593",
        "params": [
            {
                "color": "61a3b9f3f5015805829cd79e",
                "pattern": "line",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    }
                ]
            }
        ],
        "frontImage": "front.jpg",
        "backImage": "back.jpg",
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
        "photos": [
            "photo-1.jpg",
            "photo-2.jpg",
            "photo-3.jpg",
            "photo-4.jpg"
        ],
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
                "color": "61a3b9f3f5015805829cd79e",
                "secondColor": "61a3b9f3f5015805829cd79e",
                "pattern": "cell || goose || line || print || chameleon",
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
                "color": "61a3b9f3f5015805829cd795",
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
        "frontImage": "front.jpg",
        "backImage": "back.jpg",
        "aboutRU": "test",
        "aboutEN": "test",
        "aboutUK": "test",
        "compoRU": "test",
        "compoEN": "test",
        "compoUK": "test",
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
        "_id": "61a3b9f3f5015805829cd795",
        "hex": "#5C3BFE",
    },
    {
        "_id": "61a3b9f3f5015805829cd79e",
        "hex": "#FFFFFF",
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
        "hex": "#5C3BFE"
    },
    {
        "_id": "61a3b9f3f5015805829cd79e",
        "hex": "#FFFFFF"
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
        "_id": "61a7c96f29c3d72bc4a5e8d9",
        "date": "12/01/2021",
        "time": "21:13",
        "firstname": "test",
        "lastname": "test",
        "email": "minimal.wbd@gmail.com",
        "phone": "+38012 312 3123",
        "comment": "test",
        "delivery": "Новая почта (в отделение)",
        "city": "м. Суми",
        "department": "Відділення №8 (до 30 кг): просп. Михайла Лушпи, 13",
        "address": "",
        "total": "28000",
        "currency": "uah",
        "deliveryStatus": "formed",
        "userId": null,
        "cart": [
            {
                "params": [
                    {
                        "count": 2,
                        "size": "S",
                        "sizeId": "61a3ba49c9a4394f26faf591",
                        "color": "#5C3BFE",
                        "secondColor": null,
                        "colorId": "61a3b9f3f5015805829cd795",
                        "pattern": null
                    }
                ],
                "productId": "61a4afc2c63be8e71aeb81b8"
            }
        ],
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
            "productId": "61a4afc2c63be8e71aeb81b8",
            "params": [
                {
                    "count": 2,
                    "sizeId": "61a3ba49c9a4394f26faf591",
                    "secondColor": "",
                    "colorId": "61a3b9f3f5015805829cd795",
                    "pattern": ""
                }
            ],
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
                    "_id": "61a7c572feea7919a41ea77f",
                    "productId": "61a4afc2c63be8e71aeb81b8",
                    "params": [
                        {
                            "_id": "61a7c572feea7919a41ea780",
                            "count": 2,
                            "size": "S",
                            "sizeId": "61a3ba49c9a4394f26faf591",
                            "color": "#FFFFFF",
                            "secondColor": "#5C3BFE",
                            "colorId": "61a3b9f3f5015805829cd79e",
                            "pattern": "goose"
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
                "color": "61a3b9f3f5015805829cd79e",
                "secondColor": "61a3b9f3f5015805829cd795",
                "pattern": "goose",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 7,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": "61a3b9f3f5015805829cd795",
                "sizes": [
                    {
                        "amount": 5,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            }
        ]
    },
    {
        "_id": "61a6280b92459c044c5db748",
        "params": [
            {
                "color": "61a3b9f3f5015805829cd79e",
                "pattern": "line",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
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
                "color": "61a3b9f3f5015805829cd79e",
                "secondColor": "61a3b9f3f5015805829cd795",
                "pattern": "cell || goose || line || print || chameleon",
                "sizes": [
                    {
                        "amount": 10,
                        "size": "61a3ba2e730503f53b36e63f"
                    },
                    {
                        "amount": 7,
                        "size": "61a3ba49c9a4394f26faf591"
                    }
                ]
            },
            {
                "color": "61a3b9f3f5015805829cd795",
                "sizes": [
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
