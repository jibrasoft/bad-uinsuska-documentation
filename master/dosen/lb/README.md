# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Dosen LB API Spec

## Authentication
No authentication needed to use this API

## Get Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen/lb/{nip}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "nip" : "string",
         "idh" : "string",
         "idj" : "string|null",
         "nama" : "string",
         "nidn_nup" : "string",
         "golongan_jabatan" : "string",
         "email" : "string",
         "homebase" : {
             "idh": "string",
             "nama": "string",
             "tgl_update": "datetime",
             "l": "integer",
             "p": "integer",
             "jlh": "integer"
         },
         "jabatan" : {
              "idj" : "string",
              "nama" : "string",
              "sks" : "integer"
         }
    }
}
```

## List Dosen
Request :
- Method : GET
- Endpoint : `/api/lb/dosen`
- Header :
    - Accept: application/json
- Query Param :
    - idh : string
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "nip" : "string",
             "idh" : "string",
             "idj" : "string|null",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
             "homebase" : {
                 "idh": "string",
                 "nama": "string",
                 "tgl_update": "datetime",
                 "l": "integer",
                 "p": "integer",
                 "jlh": "integer"
             },
             "jabatan" : {
                  "idj" : "string",
                  "nama" : "string",
                  "sks" : "integer"
             }
        },
        {
             "nip" : "string",
             "idh" : "string",
             "idj" : "string|null",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
             "homebase" : {
                 "idh": "string",
                 "nama": "string",
                 "tgl_update": "datetime",
                 "l": "integer",
                 "p": "integer",
                 "jlh": "integer"
             },
            "jabatan" : {
                  "idj" : "string",
                  "nama" : "string",
                  "sks" : "integer"
            }
        }
    ]
}
```