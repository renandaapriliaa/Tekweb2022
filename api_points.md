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


**Menghapus data anggota**
```
DELETE: /users/[1]

response:
true   

## Portfolios ##
**Menampilkan semua data portfolio**
```
GET: /portfolios

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

**Menampilkan semua data portofolio oleh penulis tertentu**
```
GET: /portfolios/1

response:
[

{
    "id": "1",
    "Nama": "Renanda Aprilia Nurjanah",
    "Avatar": "https://renandaapriliaa.my.id/images/img.jpg",
    "Bio": "College Student & Photography Enthusiast from Indonesia",
    "Content": "Holla felas, My Name is Renanda Aprilia Nurjanah, you can call me renan,rena,etc. I'm 21        years old, single happy and free :). Now, i study at Ahmad Dahlan Univeresity in major Information        System on term 4. My hobby is singing and also taking some random p"
}
]


**Menampilkan data portfolio berdasarkan id**
```
GET: /portofolios/[id]

response:

{
          "id"           : "",
          "author_id"    : "",
          "author_name"  : "",
          "title"        : "",
          "description"  : "",
          "thumbnail_url": "",
          "technologies" : ["", "", ...],
          "project_url"  : "",
          "project_start": "",
          "project_end"  : ""
}
```

**Menambahkan data portofolio**
```
POST: /portfolios

data:
{
     "author_name"  : "",
     "title"        : "",
     "description"  : "",
     "thumbnail_url": "",
     "technologies" : ["", "", ...],
     "project_url"  : "",
     "project_start": "",
     "project_end"  : ""
}



