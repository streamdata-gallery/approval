---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set approval status of viewing slot on multi viewing appointment
  version: 1.0.0
  description: Set approval status of viewing slot on multi viewing appointment.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/viewing/{id}/recordslotapproval/{viewingSlotId}:
    put:
      summary: Set approval status of viewing slot on multi viewing appointment
      description: Set approval status of viewing slot on multi viewing appointment.
      operationId: Viewing_RecordViewingSlotApprovalByidByviewingSlotIdBystatus
      x-api-path-slug: apiviewingidrecordslotapprovalviewingslotid-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: status
      - in: path
        name: viewingSlotId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Approval
      - Status
      - Of
      - Viewing
      - Slot
      - "On"
      - Multi
      - Viewing
      - Appointment
  /api/people/{id}/updateservicetypes:
    post:
      summary: "Update the service types by PersonId\r\nThis cannot be used internally
        as they do not have the right to move status up to to approved \r\nOnly the
        client does"
      description: "Update the service types by personid\r\nthis cannot be used internally
        as they do not have the right to move status up to to approved \r\nonly the
        client does."
      operationId: People_UpdateServiceTypesByidByServiceTypes
      x-api-path-slug: apipeopleidupdateservicetypes-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: ServiceTypes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Types
      - By
      - "PersonId\r\nThis"
      - Cannot
      - Be
      - Used
      - Internally
      - As
      - They
      - Do
      - Not
      - Have
      - Right
      - To
      - Move
      - Status
      - Up
      - To
      - To
      - Approved
      - Only
      - Client
      - Does
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