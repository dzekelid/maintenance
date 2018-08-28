swagger: "2.0"
x-collection-name: Site24x7
x-complete: 1
info:
  title: User Group API
  description: the-user-group-api-
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maintenance/{maintenance_id}:
    get:
      summary: Retrieve Maintenance
      description: Retrieve configuration of a Scheduled Maintenance.
      operationId: retrieve-maintenance
      x-api-path-slug: maintenancemaintenance-id-get
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Maintenance
    delete:
      summary: Delete Maintenance
      description: Delete an existing Scheduled Maintenance.
      operationId: delete-maintenance
      x-api-path-slug: maintenancemaintenance-id-delete
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Maintenance