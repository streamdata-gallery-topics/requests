---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeSpotInstanceRequests:
    get:
      summary: Describe Spot Instance Requests
      description: Describes the Spot instance requests that belong to your account.
      operationId: describespotinstancerequests
      x-api-path-slug: actiondescribespotinstancerequests-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: Filters the results by the specified Availability Zone
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EndTime
        description: The date and time, up to the current date, from which to stop
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InstanceType.N
        description: Filters the results by the specified instance types
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of results
        type: string
      - in: query
        name: ProductDescription.N
        description: Filters the results by the specified basic product descriptions
        type: string
      - in: query
        name: StartTime
        description: The date and time, up to the past 90 days, from which to start
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Instance Requests
  /?Action=DescribeSpotFleetRequests:
    get:
      summary: Describe Spot Fleet Requests
      description: Describes your Spot fleet requests.
      operationId: describespotfleetrequests
      x-api-path-slug: actiondescribespotfleetrequests-get
      responses:
        200:
          description: OK
      tags:
      - Sport Fleet Requests
---