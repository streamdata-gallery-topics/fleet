---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Request Spot Fleet
  version: 1.0.0
  description: Creates a Spot fleet request.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelSpotFleetRequests:
    get:
      summary: Cancel Spot Fleet Requests
      description: Cancels the specified Spot fleet requests.
      operationId: cancelspotfleetrequests
      x-api-path-slug: actioncancelspotfleetrequests-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
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
        name: SpotFleetRequestId
        description: The ID of the Spot fleet request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet
  /?Action=DescribeSpotFleetInstances:
    get:
      summary: Describe Spot Fleet Instances
      description: Describes the running instances for the specified Spot fleet.
      operationId: describespotfleetinstances
      x-api-path-slug: actiondescribespotfleetinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: EventType
        description: The type of events to describe
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
        name: SpotFleetRequestId
        description: The ID of the Spot fleet request
        type: string
      - in: query
        name: StartTime
        description: The starting date and time for the events, in UTC format (for
          example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet Instance
  /?Action=DescribeSpotFleetRequestHistory:
    get:
      summary: Describe Spot Fleet Request History
      description: Describes the events for the specified Spot fleet request during
        the specified time.
      operationId: describespotfleetrequesthistory
      x-api-path-slug: actiondescribespotfleetrequesthistory-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
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
        name: SpotFleetRequestId.N
        description: The IDs of the Spot fleet requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet Request History
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
  /?Action=ModifySpotFleetRequest:
    get:
      summary: Modify Spot Fleet Request
      description: Modifies the specified Spot fleet request
      operationId: modifyspotfleetrequest
      x-api-path-slug: actionmodifyspotfleetrequest-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: SpotFleetRequestConfig
        description: The configuration for the Spot fleet request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet
  /?Action=RequestSpotFleet:
    get:
      summary: Request Spot Fleet
      description: Creates a Spot fleet request.
      operationId: requestspotfleet
      x-api-path-slug: actionrequestspotfleet-get
      parameters:
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 CIDR block for your subnet
        type: string
      - in: query
        name: SubnetId
        description: The ID of your subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet
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