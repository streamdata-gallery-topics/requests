---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 PUT Bucket requestPayment
  version: 1.0.0
  description: This implementation of the PUT operation uses therequestPayment subresource
    to set the request paymentconfiguration of a bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ?requestPayment:
    get:
      summary: GET Bucket requestPayment
      description: This implementation of the GET operation uses therequestPayment
        subresource to return the request paymentconfiguration of a bucket
      operationId: get-bucket-requestpayment
      x-api-path-slug: requestpayment-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - RequestPayment
    put:
      summary: PUT Bucket requestPayment
      description: This implementation of the PUT operation uses therequestPayment
        subresource to set the request paymentconfiguration of a bucket
      operationId: put-bucket-requestpayment
      x-api-path-slug: requestpayment-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - RequestPayment
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