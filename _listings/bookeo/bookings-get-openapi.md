---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Retrieve bookings
  version: 1.0.0
  description: |-
    Retrieve existing bookings
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time booked and/or time of the last change.
     To filter by time booked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by product id.
     <p/>
     Do not use this method to periodically poll for new/changed bookings. Use webhooks (see API general documentation) instead.
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bookings:
    get:
      summary: Retrieve bookings
      description: |-
        Retrieve existing bookings
         The result is limited by the permissions of the apiKey.
         <p/>
         It is possible to filter by time booked and/or time of the last change.
         To filter by time booked, the parameters startTime and endTime are required.
         To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
         It is possible to filter by both at the same time. At least one of the two filters must be used.
         <p/>
         It is further possible to filter by product id.
         <p/>
         Do not use this method to periodically poll for new/changed bookings. Use webhooks (see API general documentation) instead.
      operationId: getBookings
      x-api-path-slug: bookings-get
      parameters:
      - in: query
        name: endTime
        description: if specified, only include bookings that start on or before this
          time
      - in: query
        name: expandCustomer
        description: if true, the full details of the customer are included (provided
          the application has read permission over the customer)
      - in: query
        name: expandParticipants
        description: if true, full details of the participants are included (provided
          the application has read permission over the participant)
      - in: query
        name: includeCanceled
        description: if true, canceled bookings are included
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: lastUpdatedEndTime
        description: if specified, only include bookings that were last changed (or
          created) on or before this time
      - in: query
        name: lastUpdatedStartTime
        description: if specified, only include bookings that were last changed (or
          created) on or after this time
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: productId
        description: if not specified, include bookings for all products
      - in: query
        name: startTime
        description: if specified, only include bookings that start on or after this
          time
      responses:
        200:
          description: OK
      tags:
      - Bookings
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