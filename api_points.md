# API Points #
## Users ##
**Menampilkan data semua pengguna**
```
GET: /users

response:[
{
    "id": "2",
    "Title": "Renanda's Portfolio",
    "Avatar_url": "https://github.com/renandaapriliaa/Tekwe",
    "Motto": "Sebuah perjalanan ilmu menjelajah kode. ",
    "Ig_url": "https://www.instagra",
    "Github_url": "https://github.com/r",
    "Linkedin_url": ""
},
{
    "id": "3",
    "Title": "Oxtella's Portfolio",
    "Avatar_url": "https://github.com/renandaapriliaa/Tekwe",
    "Motto": "Sebuah perjalanan ilmu menjelajah kode. ",
    "Ig_url": "https://www.instagra",
    "Github_url": "https://github.com/r",
    "Linkedin_url": ""
}
]
```

**Menampilkan data semua pengguna dengan id tertentu**
```
GET: /users/[2]

response:
{
    "id": "2",
    "Title": "Renanda's Portfolio",
    "Avatar_url": "https://github.com/renandaapriliaa/Tekwe",
    "Motto": "Sebuah perjalanan ilmu menjelajah kode. ",
    "Ig_url": "https://www.instagra",
    "Github_url": "https://github.com/r",
    "Linkedin_url": ""
}
 ```
 
 **Menambahkan data pengguna**
 ```
 POST: /users
 
 data:
 {
    "Title": "Oxtella's Portfolio",
    "Avatar_url": "https://github.com/renandaapriliaa/Tekwe",
    "Motto": "Sebuah perjalanan ilmu menjelajah kode. ",
    "Ig_url": "https://www.instagra",
    "Github_url": "https://github.com/r",
    "Linkedin_url": ""
}

response:
true 
```

**Edit data pengguna**
```
PUT: /users

data:
{
    "Title": "Renanda's Portfolio",
    "Avatar_url": "https://github.com/renandaapriliaa/Tekwe",
    "Motto": "Sebuah perjalanan ilmu menjelajah kode. ",
    "Ig_url": "https://www.instagra",
    "Github_url": "https://github.com/r",
    "Linkedin_url": ""
}
 
 
response:
true   
```

**Menghapus data anggota**
```
DELETE: /users/[1]

response:
true   
```

## Portfolios ##
**Menampilkan semua data portfolio**
```
GET: /portfolio

response: [
{
    "id": "1",
    "Nama": "Renanda Aprilia Nurjanah",
    "Avatar": "https://renandaapriliaa.my.id/images/img.jpg",
    "Bio": "College Student & Photography Enthusiast from Indonesia",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21       years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information         System on term 4. My hobby is singing and also taking some random p"
},
{
    id": "2",
    "Nama": "Oxella Martha",
    "Avatar": "https://cdn1-production- imagesly.akamaized.net/K6aqbbvhHZ4h5Xvk2fz8UUvHaYg=/1200x1200/smart/filter",
    "Bio": "Artist",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21        years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information        System on term 4. My hobby is singing and also taking some random p"
}
]
```

**Menampilkan data portfolio berdasarkan id**
```
GET: /portofolio/[1]

response:

{
    "id": "1",
    "Nama": "Renanda Aprilia Nurjanah",
    "Avatar": "https://renandaapriliaa.my.id/images/img.jpg",
    "Bio": "College Student & Photography Enthusiast from Indonesia",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21       years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information         System on term 4. My hobby is singing and also taking some random p"
}
```

**Menambahkan data portofolio**
```
POST: /portfolio

data:
{
    "Nama": "Zee Mark",
    "Avatar": "https://cdn1-production-images-            kly.akamaized.net/K6aqbbvhHZ4h5Xvk2fz8UUvHaYg=/1200x1200/smart/filter",
    "Bio": "Artist",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21        years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information        System on term 4. My hobby is singing and also taking some random p"
}

response:
true
```

**Edit data portofolio**
```
PUT: /portofolio

data:
{
   
    "Nama": "Zoe Martin",
    "Avatar": "https://cdn1-production-images-  kly.akamaized.net/K6aqbbvhHZ4h5Xvk2fz8UUvHaYg=/1200x1200/smart/filter",
    "Bio": "Artist",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21        years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information        System on term 4. My hobby is singing and also taking some random p"

}
 
response:
true   
```

**Menghapus data pada portofolio**
```
DELETE: /potofolio/[3]

response:
true
```

## Articles ##
**Menampilkan data semua articles**
```
GET: /articles

response:[
    {
    "id": "1",
    "Thumbnail": "https://renandaapriliaa.my.id/images/artc1.jpeg",
    "Title": "Photography Enthusiast",
    "Content": "Here is several things why Photography is fun."
},
    {
    "id": "2",
    "Thumbnail": "https://renandaapriliaa.my.id/images/artc2.jpeg",
    "Title": "Yogyakarta",
    "Content": "Jogja The Never Ending Asia"
},
    {
    "id": "3",
    "Thumbnail": "https://images.unsplash.com/photo-1515879218367-8466d910aaa4?        ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=869       &q=80",
    "Title": "Card title",
    "Content": "Some quick example text to build on the card title"
},
    {
    "id": "4",
    "Thumbnail": "https://renandaapriliaa.my.id/images/artc1.jpeg",
    "Title": "Photography Enthusiast",
    "Content": "Here is several things why Photography is fun."
},
    {
    "id": "5",
    "Thumbnail": "https://renandaapriliaa.my.id/images/artc1.jpeg",
    "Title": "Photography Enthusiast",
    "Content": "Here is several things why Photography is fun."
    }
]
```

**Menampilkan data semua articles dengan id tertentu**
```
GET: /artciles/[1]

response:
{
"id": "1",
"Thumbnail": "https://renandaapriliaa.my.id/images/artc1.jpeg",
"Title": "Photography Enthusiast",
"Content": "Here is several things why Photography is fun."
}
 ```
 
 **Menambahkan data articles**
 ```
 POST: /articles
 
 data:
 {
    "Thumbnail": "https://renandaapriliaa.my.id/images/artc1.jpeg",
    "Title": "Photography Enthusiast",
    "Content": "Here is several things why Photography is fun."
}

response:
true 
```

**Edit data articles**
```
PUT: /articles

data:
{
"Thumbnail": "https://renandaapriliaa.my.id/images/artc2.jpeg",
"Title": "Photography Enthusiast",
"Content": "Here is several things why Photography is fun."
}
 
response:
true   
```

**Menghapus data articles**
```
DELETE: /articles/[6]

response:
true   
 



