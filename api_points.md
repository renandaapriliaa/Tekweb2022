# API Points #
## Users ##
**Menampilkan data semua pengguna**
```
GET: /users

response:
[
    {
       "id"           : "",
       "name"         : "",
       "motto"        : "",
       "ig_url"       : "",
       "gh_url"       : "",
       "ld_url"       : "",
       "avatar_url"   : "",
       
   },
   ...
]
```

**Menampilkan data semua pengguna dengan id tertentu**
```
GET: /users/[id]

response:
{
       "id"           : "",
       "name"         : "",
       "motto"        : "",
       "ig_url"       : "",
       "gh_url"       : "",
       "ld_url"       : "",
       "avatar_url"   : "",
       
 }
 ```
 
 **Menambahkan data pengguna**
 ```
 POST: /users
 
 data:
 {
        "nama"        : "",
        "motto"       : "",
        "ig_url"      : "",
        "gh_url"      : "",
        "ld_url"      : "",
        "avatar_url"  : "",
}

response:
true    // if success
false   // if failure
```

**Edit data pengguna**
```
PUT: /users

data:
{
       "id"           : "",
       "name"         : "",
       "motto"        : "",
       "ig_url"       : "",
       "gh_url"       : "",
       "ld_url"       : "",
       "avatar_url"   : "",
       
 }
 
 
response:
true    // if success
false   // if failure
```

**Menghapus data anggota**
```
DELETE: /users/[id]

response:
true    // if success
false   // if failure
```

## Portfolios ##
**Menampilkan semua data portfolio**
```
GET: /portfolios

response:
[
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
     },
     ...
]
```

**Menampilkan semua data portofolio oleh penulis tertentu**
```
GET: /portfolios/author/author_id

response:
[

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
     },
     ...
]
```

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



