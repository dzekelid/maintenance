{
  "info": {
    "name": "Amazon RDS API Apply Pending Maintenance Action",
    "_postman_id": "9cedacc9-28a3-42fb-8cac-fe2afce9abba",
    "description": "Applies a pending maintenance action to a resource (for example, to a DB instance).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "e939fb2c-9ad1-4b88-ab32-1b92f58208d3",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c32ef0ff-f8c7-477e-9946-1c8b9e394696"
            }
          ]
        }
      ]
    }
  ]
}