---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe Pending Maintenance Actions
  version: 1.0.0
  description: Returns a list of resources (for example, DB instances) that have at
    least one pending maintenance action.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ApplyPendingMaintenanceAction:
    get:
      summary: Apply Pending Maintenance Action
      description: Applies a pending maintenance action to a resource (for example,
        to a DB instance).
      operationId: applypendingmaintenanceaction
      x-api-path-slug: actionapplypendingmaintenanceaction-get
      parameters:
      - in: query
        name: ApplyAction
        description: The pending maintenance action to apply to this resource
        type: string
      - in: query
        name: OptInType
        description: A value that specifies the type of opt-in request, or undoes
          an opt-in request
        type: string
      - in: query
        name: ResourceIdentifier
        description: The RDS Amazon Resource Name (ARN) of the resource that the       pending
          maintenance action applies to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance Actions
  /?Action=DescribePendingMaintenanceActions:
    get:
      summary: Describe Pending Maintenance Actions
      description: Returns a list of resources (for example, DB instances) that have
        at least one pending maintenance action.
      operationId: describependingmaintenanceactions
      x-api-path-slug: actiondescribependingmaintenanceactions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more resources to return pending
          maintenance actions for
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribePendingMaintenanceActions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ResourceIdentifier
        description: The ARN of a resource to return pending maintenance actions for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance Actions
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---