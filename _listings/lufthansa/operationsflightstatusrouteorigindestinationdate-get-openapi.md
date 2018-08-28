---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Flight Status by Route
  version: "1.0"
  description: Status of flights between a given origin and destination on a given
    date.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /operations/schedules/{origin}/{destination}/{fromDateTime}:
    get:
      summary: Flight Schedules
      description: Scheduled flights between given airports on a given date.
      operationId: OperationsSchedulesFromDateTimeByOriginAndDestinationGet
      x-api-path-slug: operationsschedulesorigindestinationfromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: destination
        description: Destination airport
      - in: query
        name: directFlights
        description: Show only direct flights (false=0, true=1)
      - in: path
        name: fromDateTime
        description: Local departure date and optionally departure time (YYYY-MM-DD
          or YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Schedules
      - Origin
      - Destination
      - FromDateTime
  /operations/flightstatus/route/{origin}/{destination}/{date}:
    get:
      summary: Flight Status by Route
      description: Status of flights between a given origin and destination on a given
        date.
      operationId: OperationsFlightstatusRouteDateByOriginAndDestinationGet
      x-api-path-slug: operationsflightstatusrouteorigindestinationdate-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD) in local time of departure airport
      - in: path
        name: destination
        description: 3-letter IATA airport code (e
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: 3-letter IATA airport (e
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Route
      - Origin
      - Destination
      - Date
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