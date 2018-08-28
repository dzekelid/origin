---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez To save or edit the Group additional info i.e. the Origin and Grade.
  version: 1.0.0
  description: To save or edit the group additional info i.e. the origin and grade..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/saveadditionalinfo:
    put:
      summary: To save or edit the Group additional info i.e. the Origin and Grade.
      description: To save or edit the group additional info i.e. the origin and grade..
      operationId: Group_SaveAdditionalInfoByidBysaveAdditionalInfoDataContract
      x-api-path-slug: apigroupidsaveadditionalinfo-put
      parameters:
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveAdditionalInfoDataContract
        description: The additional info to set on the group i
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Save
      - Edit
      - Group
      - Additional
      - Info
      - I
      - E
      - ""
      - Origin
      - Grade
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