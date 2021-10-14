# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
SKS Jabatan API Spec

## Authentication
No authentication needed to use this API

## Get Jabatan
Request :
- Method : GET
- Endpoint : `/api/jabatan/{idj}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "idj" : "string",
         "nama" : "string",
         "sks" : "integer"
    }
}
```

## List Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen`
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
            "idj" : "string",
            "nama" : "string",
            "sks" : "integer"
        },
        {
            "idj" : "string",
            "nama" : "string",
            "sks" : "integer"
        }
    ]
}
```