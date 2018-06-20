---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeMaintenanceStartTime:
    get:
      summary: Describe Maintenance Start Time
      description: |-
        Returns your gateway's weekly maintenance start time including the day and time of
                 the week.
      operationId: describeMaintenanceStartTime
      x-api-path-slug: actiondescribemaintenancestarttime-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
        200:
          description: OK
      tags:
      - Maintenance
  /?Action=UpdateMaintenanceStartTime:
    get:
      summary: Update Maintenance Start Time
      description: |-
        Updates a gateway's weekly maintenance start time information, including day and time
                 of the week.
      operationId: updateMaintenanceStartTime
      x-api-path-slug: actionupdatemaintenancestarttime-get
      parameters:
      - in: query
        name: DayOfWeek
        description: The maintenance start time day of the week represented as an
          ordinal number from 0 to 6,          where 0 represents Sunday and 6 Saturday
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: HourOfDay
        description: The hour component of the maintenance start time represented
          as            hh, where hh is the hour (00 to 23)
        type: string
      - in: query
        name: MinuteOfHour
        description: The minute component of the maintenance start time represented
          as            mm, where mm is the minute (00 to 59)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
---