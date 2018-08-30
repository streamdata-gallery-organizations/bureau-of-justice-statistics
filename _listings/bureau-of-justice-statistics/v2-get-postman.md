{
  "info": {
    "name": "National Crime Victimization Survey (NCVS) API Get",
    "_postman_id": "7ec5e50d-4cf2-4c0e-8975-68f6a4dc6b4b",
    "description": "Returns a list of available datasets and data types they are available in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "66e9a711-9bd0-4adf-976d-03e20901ffaa",
      "name": "getV2",
      "request": {
        "url": "http://www.bjs.gov/bjs/ncvs/v2/",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of available datasets and data types they are available in."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "25979c6c-225b-4a8c-bc0c-b8f9abddc0de"
        }
      ]
    }
  ]
}