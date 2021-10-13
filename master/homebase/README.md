# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Homebase API Spec

## Authentication
No authentication needed to use this API

## Get Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen/homebase/{idh}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
          "nma": "string",
          "tgl_update": "datetime",
          "idh": "string",
          "l": "integer",
          "p": "integer",
          "jlh": "integer"
    }
}
```

## List Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen/homebase`
- Header :
    - Accept: application/json
Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
            "nma": "string",
            "tgl_update": "datetime",
            "idh": "string",
            "l": "integer",
            "p": "integer",
            "jlh": "integer"
        },
        {
            "nma": "string",
            "tgl_update": "datetime",
            "idh": "string",
            "l": "integer",
            "p": "integer",
            "jlh": "integer"
        }
    ]
}
```