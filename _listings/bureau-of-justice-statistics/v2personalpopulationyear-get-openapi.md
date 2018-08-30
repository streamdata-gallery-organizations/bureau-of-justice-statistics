---
swagger: "2.0"
x-collection-name: Bureau of Justice Statistics
x-complete: 0
info:
  title: National Crime Victimization Survey (NCVS) API Get Personal Population Year
  description: Returns the personal population of reported incidents.
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
  v2/household/fields/:
    get:
      summary: Get Household Fields
      description: Returns a description of the fields/columns used returned in the
        household data sets.
      operationId: getV2HouseholdFields
      x-api-path-slug: v2householdfields-get
      responses:
        200:
          description: OK
      tags:
      - Household
      - Fields
  v2/household/population/{year}:
    get:
      summary: Get Household Population Year
      description: Returns the personal population of reported incidents.
      operationId: getV2HouseholdPopulationYear
      x-api-path-slug: v2householdpopulationyear-get
      parameters:
      - in: query
        name: format
        description: Format the data will be provided in
      - in: query
        name: year
        description: Year will limit the data to only values that occurred the given
          year
      responses:
        200:
          description: OK
      tags:
      - Household
      - Population
      - Year
  v2/household/{year}:
    get:
      summary: Get Household Year
      description: Returns the household counts of reported incidents
      operationId: getV2HouseholdYear
      x-api-path-slug: v2householdyear-get
      parameters:
      - in: query
        name: format
        description: Format the data will be provided in
      - in: query
        name: year
        description: Year will limit the data to only values that occurred the given
          year
      responses:
        200:
          description: OK
      tags:
      - Household
      - Year
  v2/personal/fields/:
    get:
      summary: Get Personal Fields
      description: Returns a description of the fields/columns used returned in the
        personal data sets.
      operationId: getV2PersonalFields
      x-api-path-slug: v2personalfields-get
      responses:
        200:
          description: OK
      tags:
      - Personal
      - Fields
  v2/personal/population/{year}:
    get:
      summary: Get Personal Population Year
      description: Returns the personal population of reported incidents.
      operationId: getV2PersonalPopulationYear
      x-api-path-slug: v2personalpopulationyear-get
      parameters:
      - in: query
        name: format
        description: Format the data will be provided in
      - in: query
        name: year
        description: Year will limit the data to only values that occurred the given
          year
      responses:
        200:
          description: OK
      tags:
      - Personal
      - Population
      - Year
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