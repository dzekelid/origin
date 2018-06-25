---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: Origin
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Public Retrieve all flights
  x-api-slug: lh-public
  description: Retrieve a list of all possible flights (both direct and connecting)
    between two airports on a given date. Routes are available for today and up to
    days in the future.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//cargo/getRoute/{origin}-{destination}/{fromDate}/{productCode}
  tags: Cargo,GetRoute,Origin,Destination,FromDate,ProductCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/cargogetrouteorigindestinationfromdateproductcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/cargogetrouteorigindestinationfromdateproductcode-get-openapi.md
- name: LH Public Seat Maps
  x-api-slug: lh-public
  description: Cabin layout and seat characteristics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//offers/seatmaps/{flightNumber}/{origin}/{destination}/{date}/{cabinClass}
  tags: Offers,Seatmaps,FlightNumber,Origin,Destination,Date,CabinClass
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/offersseatmapsflightnumberorigindestinationdatecabinclass-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/offersseatmapsflightnumberorigindestinationdatecabinclass-get-openapi.md
- name: LH Public Flight Status by Route
  x-api-slug: lh-public
  description: Status of flights between a given origin and destination on a given
    date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//operations/flightstatus/route/{origin}/{destination}/{date}
  tags: Operations,Flightstatus,Route,Origin,Destination,Date
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/operationsflightstatusrouteorigindestinationdate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/operationsflightstatusrouteorigindestinationdate-get-openapi.md
- name: LH Public Flight Schedules
  x-api-slug: lh-public
  description: Scheduled flights between given airports on a given date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//operations/schedules/{origin}/{destination}/{fromDateTime}
  tags: Operations,Schedules,Origin,Destination,FromDateTime
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/operationsschedulesorigindestinationfromdatetime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/operationsschedulesorigindestinationfromdatetime-get-openapi.md
- name: LH Public
  x-api-slug: lh-public
  description: Book your flights to Germany, Italy, UK or France online at attractive
    low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Origin
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/origin/master/_listings/lufthansa/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/lufthansa
- type: x-twitter
  url: https://twitter.com/lufthansa
- type: x-website
  url: http://lufthansa.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---