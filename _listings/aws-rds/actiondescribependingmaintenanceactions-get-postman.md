{
  "info": {
    "name": "Amazon RDS API Describe Pending Maintenance Actions",
    "_postman_id": "35014b7c-3d8c-415f-8afe-5b3e4c7d825f",
    "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "248ee564-e526-4f73-87bc-0ce06d6a2d4c",
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
              "id": "ee2c834f-6797-4b84-91e6-8aae7bab9bd2"
            }
          ]
        },
        {
          "id": "598d5312-be37-444d-aae8-70dc7c0e89ae",
          "name": "describependingmaintenanceactions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePendingMaintenanceActions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbdcb40f-f034-4cc6-96a5-c65c7c81fb04"
            }
          ]
        }
      ]
    }
  ]
}