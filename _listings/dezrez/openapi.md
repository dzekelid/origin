swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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