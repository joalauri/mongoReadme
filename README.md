```
use ecommerce;
```

```js
db.products.insertOne({
productId: "MCO967705850",
    title: "Laptop Asus M515da Gris 15.6 , Amd Ryzen 5 3500u  16gb De Ram 1tb Hdd 256gb Ssd, Amd Radeon Rx Vega 8 (ryzen 2000/3000) 1920x1080px Windows 10",
    price: 1999900,
    stock: 7,
    thumbnail: "http://http2.mlstatic.com/D_894333-MLA51165023913_082022-F.jpg"
});



res:
{
  acknowledged: true,
  insertedId: ObjectId("639a3f149f3d4271fca954f0")
}
```

```js
db.messages.insertOne({
id: "isajdh12132jkji",
message: "esto es un mensaje de prueba"
});


res: {
  acknowledged: true,
  insertedId: ObjectId("639a41909f3d4271fca954f2")
}
```
```js
db.messages.find()

res:[
  {
    _id: ObjectId("639a41909f3d4271fca954f2"),
    id: 'isajdh12132jkji',
    message: 'esto es un mensaje de prueba'
  }
]
```



```js
db.products.insertMany([
{
    productId: "MCO657791576",
    title: "Torre Cpu Gamer Ryzen 7 5700g Vega 8 1tb 16gb Pc",
    price: 3049900,
    stock: 1,
    thumbnail: "http://http2.mlstatic.com/D_661268-MCO47189663977_082021-F.jpg"
  },
  {
    productId: "MCO879442053",
    title: "Kit De Teclado Y Mouse Inalámbrico Logitech Mk235 Español De Color Negro",
    price: 95000,
    stock: 11,
    thumbnail: "http://http2.mlstatic.com/D_961801-MLA48377493379_112021-F.jpg"
  },
  {
    productId: "MCO964679805",
    title: "Disco SólproductIdo Ssd Interno Kingston Sa400s37/240g 240gb Negro",
    price: 103322,
    stock: 23,
    thumbnail: "http://http2.mlstatic.com/D_804287-MLA49587128302_042022-F.jpg"
  },
  {
    productId: "MCO936445457",
    title: "Laptop Hp 240 G7 Gris 14 , Intel Celeron N4020 8gb De Ram 1tb Hdd, Intel Uhd Graphics 600 1366x768px Windows 10 Home",
    price: 905900,
    stock: 6,
    thumbnail: "http://http2.mlstatic.com/D_679578-MLA49695293979_042022-F.jpg"
  },
  {
    productId: "MCO939489276",
    title: "Disco SólproductIdo Ssd Interno Kingston Sa400s37/480g 480gb Negro",
    price: 160000,
    stock: 3,
    thumbnail: "http://http2.mlstatic.com/D_751939-MLA46221843872_052021-F.jpg"
  },
  {
    productId: "MCO818960598",
    title: "Pc Computador Gamer Amd Ryzen 7 5700g Ssd 240 Hdd 1tb Ram 16",
    price: 3859900,
    stock: 1,
    thumbnail: "http://http2.mlstatic.com/D_862652-MCO47807316125_102021-F.jpg"
  },
  {
    productId: "MCO943311946",
    title: "Monitor Gamer Samsung F22t35 Led 22n Dark Blue Gray 100v/240v",
    price: 524739,
    stock: 3,
    thumbnail: "http://http2.mlstatic.com/D_796587-MLA46165231779_052021-F.jpg"
  },
  {
    productId: "9cdffcf8-8d9f-40a9-a6d0-2d63e037944d",      
    title: "Laptop Dell Inspiron 3505 Gris 15.6 , Amd Ryzen 5 3450u 16gb De Ram 1tb Hdd 256gb Ssd",
    price: 2059900,
    stock: 25,
    thumbnail: "https://http2.mlstatic.com/D_921052-MLA47215256520_082021-O.jpg"
  }
]);


res: 


{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId("639a44e09f3d4271fca954f3"),
    '1': ObjectId("639a44e09f3d4271fca954f4"),
    '2': ObjectId("639a44e09f3d4271fca954f5"),
    '3': ObjectId("639a44e09f3d4271fca954f6"),
    '4': ObjectId("639a44e09f3d4271fca954f7"),
    '5': ObjectId("639a44e09f3d4271fca954f8"),
    '6': ObjectId("639a44e09f3d4271fca954f9"),
    '7': ObjectId("639a44e09f3d4271fca954fa")
  }
}
```




```js
ecommerce> db.products.find();
res: 
[
  {
    _id: ObjectId("639a3f149f3d4271fca954f0"),
    productId: 'MCO967705850',
    title: 'Laptop Asus M515da Gris 15.6 , Amd Ryzen 5 3500u  16gb De Ram 1tb Hdd 256gb Ssd, Amd Radeon Rx Vega 8 (ryzen 2000/3000) 1920x1080px Windows 10',
    price: 1999900,
    stock: 7,
    thumbnail: 'http://http2.mlstatic.com/D_894333-MLA51165023913_082022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f3"),
    productId: 'MCO657791576',
    title: 'Torre Cpu Gamer Ryzen 7 5700g Vega 8 1tb 16gb Pc',
    price: 3049900,
    stock: 1,
    thumbnail: 'http://http2.mlstatic.com/D_661268-MCO47189663977_082021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f4"),
    productId: 'MCO879442053',
    title: 'Kit De Teclado Y Mouse Inalámbrico Logitech Mk235 Español De Color Negro',
    price: 95000,
    stock: 11,
    thumbnail: 'http://http2.mlstatic.com/D_961801-MLA48377493379_112021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f5"),
    productId: 'MCO964679805',
    title: 'Disco SólproductIdo Ssd Interno Kingston Sa400s37/240g 240gb Negro',
    price: 103322,
    stock: 23,
    thumbnail: 'http://http2.mlstatic.com/D_804287-MLA49587128302_042022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f6"),
    productId: 'MCO936445457',
    title: 'Laptop Hp 240 G7 Gris 14 , Intel Celeron N4020 8gb De Ram 1tb Hdd, Intel Uhd Graphics 600 1366x768px Windows 10 Home',
    price: 905900,
    stock: 6,
    thumbnail: 'http://http2.mlstatic.com/D_679578-MLA49695293979_042022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f7"),
    productId: 'MCO939489276',
    title: 'Disco SólproductIdo Ssd Interno Kingston Sa400s37/480g 480gb Negro',
    price: 160000,
    stock: 3,
    thumbnail: 'http://http2.mlstatic.com/D_751939-MLA46221843872_052021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f8"),
    productId: 'MCO818960598',
    title: 'Pc Computador Gamer Amd Ryzen 7 5700g Ssd 240 Hdd 1tb Ram 16',
    price: 3859900,
    stock: 1,
    thumbnail: 'http://http2.mlstatic.com/D_862652-MCO47807316125_102021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f9"),
    productId: 'MCO943311946',
    title: 'Monitor Gamer Samsung F22t35 Led 22n Dark Blue Gray 100v/240v',
    price: 524739,
    stock: 3,
    thumbnail: 'http://http2.mlstatic.com/D_796587-MLA46165231779_052021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954fa"),
    productId: '9cdffcf8-8d9f-40a9-a6d0-2d63e037944d',
    title: 'Laptop Dell Inspiron 3505 Gris 15.6 , Amd Ryzen 5 3450u 16gb De Ram 1tb Hdd 256gb Ssd',
    price: 2059900,
    stock: 25,
    thumbnail: 'https://http2.mlstatic.com/D_921052-MLA47215256520_082021-O.jpg'
  }
]
```
```js
db.messages.insertMany([
{
id: "i987654edfvb",
message: "testing message 1"
},
{
id: "sdghu4567f",
message: "testing message 2"
},
{
id: "hghjio98765rg",
message: "testing message 3"
},
{
id: "hjko098765rf",
message: "testing message 4"
},
{
id: "gbji8765rfgh",
message: "testing message 5"
},
{
id: "gjko9876543wsdfg",
message: "testing message 6"
},
{
id: "ghu765r4fgh",
message: "testing message 7"
},
{
id: "ghjki7654efg",
message: "testing message 8"
},
{
id: "ghji98765efg",
message: "testing message 9"
}
]);


res: 

{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId("639a45c99f3d4271fca954fb"),
    '1': ObjectId("639a45c99f3d4271fca954fc"),
    '2': ObjectId("639a45c99f3d4271fca954fd"),
    '3': ObjectId("639a45c99f3d4271fca954fe"),
    '4': ObjectId("639a45c99f3d4271fca954ff"),
    '5': ObjectId("639a45c99f3d4271fca95500"),
    '6': ObjectId("639a45c99f3d4271fca95501"),
    '7': ObjectId("639a45c99f3d4271fca95502"),
    '8': ObjectId("639a45c99f3d4271fca95503")
  }
}
```
```js
db.messages.find();
res:

[
  {
    _id: ObjectId("639a41909f3d4271fca954f2"),
    id: 'isajdh12132jkji',
    message: 'esto es un mensaje de prueba'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca954fb"),
    id: 'i987654edfvb',
    message: 'testing message 1 '
  },
  {
    _id: ObjectId("639a45c99f3d4271fca954fc"),
    id: 'sdghu4567f',
    message: 'testing message 2'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca954fd"),
    id: 'hghjio98765rg',
    message: 'testing message 3'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca954fe"),
    id: 'hjko098765rf',
    message: 'testing message 4'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca954ff"),
    id: 'gbji8765rfgh',
    message: 'testing message 5'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca95500"),
    id: 'gjko9876543wsdfg',
    message: 'testing message 6'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca95501"),
    id: 'ghu765r4fgh',
    message: 'testing message 7'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca95502"),
    id: 'ghjki7654efg',
    message: 'testing message 8'
  },
  {
    _id: ObjectId("639a45c99f3d4271fca95503"),
    id: 'ghji98765efg',
    message: 'testing message 9'
  }
]
```
```js
db.products.countDocuments();
res:
9
```
```js
db.messages.countDocuments();
res:
10
```
```js
db.products.insertOne({
productId: "MCO967705850",
    title: "Laptop Asus M515da Gris 15.6 , Amd Ryzen 5 3500u  16gb De Ram 1tb Hdd 256gb Ssd, Amd Radeon Rx Vega 8 (ryzen 2000/3000) 1920x1080px Windows 10",
    price: 1999900,
    stock: 7,
    thumbnail: "http://http2.mlstatic.com/D_894333-MLA51165023913_082022-F.jpg"
});

res:

{
  acknowledged: true,
  insertedId: ObjectId("639a3f149f3d4271fca954f0")
}
```
```js
db.products.find({price: {$lt: 500000}});
res:

[
  {
    _id: ObjectId("639a44e09f3d4271fca954f4"),
    productId: 'MCO879442053',
    title: 'Kit De Teclado Y Mouse Inalámbrico Logitech Mk235 Español De Color Negro',
    price: 95000,
    stock: 11,
    thumbnail: 'http://http2.mlstatic.com/D_961801-MLA48377493379_112021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f5"),
    productId: 'MCO964679805',
    title: 'Disco SólproductIdo Ssd Interno Kingston Sa400s37/240g 240gb Negro',
    price: 103322,
    stock: 23,
    thumbnail: 'http://http2.mlstatic.com/D_804287-MLA49587128302_042022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f7"),
    productId: 'MCO939489276',
    title: 'Disco SólproductIdo Ssd Interno Kingston Sa400s37/480g 480gb Negro',
    price: 160000,
    stock: 3,
    thumbnail: 'http://http2.mlstatic.com/D_751939-MLA46221843872_052021-F.jpg'
  }
]
```
```js
db.products.find({price: {$gte:500000,$lt:1500000}});
Res:
[
  {
    _id: ObjectId("639a44e09f3d4271fca954f6"),
    productId: 'MCO936445457',
    title: 'Laptop Hp 240 G7 Gris 14 , Intel Celeron N4020 8gb De Ram 1tb Hdd, Intel Uhd Graphics 600 1366x768px Windows 10 Home',
    price: 905900,
    stock: 6,
    thumbnail: 'http://http2.mlstatic.com/D_679578-MLA49695293979_042022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f9"),
    productId: 'MCO943311946',
    title: 'Monitor Gamer Samsung F22t35 Led 22n Dark Blue Gray 100v/240v',
    price: 524739,
    stock: 3,
    thumbnail: 'http://http2.mlstatic.com/D_796587-MLA46165231779_052021-F.jpg'
  }
]

```
```js
db.products.find({price: {$gte:600000}});
res:
[
  {
    _id: ObjectId("639a3f149f3d4271fca954f0"),
    productId: 'MCO967705850',
    title: 'Laptop Asus M515da Gris 15.6 , Amd Ryzen 5 3500u  16gb De Ram 1tb Hdd 256gb Ssd, Amd Radeon Rx Vega 8 (ryzen 2000/3000) 1920x1080px Windows 10',
    price: 1999900,
    stock: 7,
    thumbnail: 'http://http2.mlstatic.com/D_894333-MLA51165023913_082022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f3"),
    productId: 'MCO657791576',
    title: 'Torre Cpu Gamer Ryzen 7 5700g Vega 8 1tb 16gb Pc',
    price: 3049900,
    stock: 1,
    thumbnail: 'http://http2.mlstatic.com/D_661268-MCO47189663977_082021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f6"),
    productId: 'MCO936445457',
    title: 'Laptop Hp 240 G7 Gris 14 , Intel Celeron N4020 8gb De Ram 1tb Hdd, Intel Uhd Graphics 600 1366x768px Windows 10 Home',
    price: 905900,
    stock: 6,
    thumbnail: 'http://http2.mlstatic.com/D_679578-MLA49695293979_042022-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954f8"),
    productId: 'MCO818960598',
    title: 'Pc Computador Gamer Amd Ryzen 7 5700g Ssd 240 Hdd 1tb Ram 16',
    price: 3859900,
    stock: 1,
    thumbnail: 'http://http2.mlstatic.com/D_862652-MCO47807316125_102021-F.jpg'
  },
  {
    _id: ObjectId("639a44e09f3d4271fca954fa"),
    productId: '9cdffcf8-8d9f-40a9-a6d0-2d63e037944d',
    title: 'Laptop Dell Inspiron 3505 Gris 15.6 , Amd Ryzen 5 3450u 16gb De Ram 1tb Hdd 256gb Ssd',
    price: 2059900,
    stock: 25,
    thumbnail: 'https://http2.mlstatic.com/D_921052-MLA47215256520_082021-O.jpg'
  }
]
```
```js
db.products.updateMany( {},{ $set: { stock:100 }});

res:{
  acknowledged: true,
  insertedId: null,
  matchedCount: 9,
  modifiedCount: 9,
  upsertedCount: 0
}

```
```js
db.products.updateMany({price:{$gte:150000}},{ $set: { stock:0 }});
res:
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 7,
  modifiedCount: 7,
  upsertedCount: 0
}
```
```js
db.products.deleteMany({price:{$lt:300000}});
res:{ acknowledged: true, deletedCount: 3 }
```
