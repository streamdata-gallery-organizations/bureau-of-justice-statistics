---
swagger: "2.0"
x-collection-name: Bureau of Justice Statistics
x-complete: 0
info:
  title: National Crime Victimization Survey (NCVS) API Get
  description: Returns a list of available datasets and data types they are available
    in.
  version: v2
host: www.bjs.gov
basePath: /bjs/ncvs/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  v2/:
    get:
      summary: Get
      description: Returns a list of available datasets and data types they are available
        in.
      operationId: getV2
      x-api-path-slug: v2-get
      responses:
        200:
          description: OK
      tags:
      - ""
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