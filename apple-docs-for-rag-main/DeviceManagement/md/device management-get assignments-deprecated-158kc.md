

- Device Management
-  Get Assignments Deprecated

Web Service Endpoint

# Get Assignments

Get a list of assignments currently assigned to a user or device.

Device Assignment ServicesVPP License Management

Deprecated

This legacy API is currently in maintenance mode. Apple won’t add any new functionality to it.

## URL

``` source
POST https://vpp.itunes.apple.com/mdm/getAssignments
```

## HTTP Body

VppAssignmentRequest

The request for a list of assignments.

Content-Type: application/json

## Response Codes

` 200 ``OK`

VppAssignmentsResponse

`OK`

The response that contains a list of assignments.

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
{
  "adamIdStr" : "361304891",
  "clientUserIdStr" : "user1",
  "sToken" : "h40Gte9aQnZFDNM39IUkRPCsQDxBxbZB4Wy34pxefOuQkeeb3h2a5Rlopo4KDn3MrFKf4CM3OY+WGAoZ1cD6iZ6yzsMk1+5PVBNc66YS6ZQ="
}
```

```
{
  "assignments" : [ {
    "adamIdStr" : "361304891",
    "clientUserIdStr" : "user1",
    "pricingParam" : "STDQ"
  } ],
  "assignmentsInCurrentPage" : 1,
  "currentPageIndex" : 0,
  "expirationMillis" : 1860422147836,
  "location" : {
    "locationId" : 22222222222,
    "locationName" : "LocationName"
  },
  "status" : 0,
  "totalAssignments" : 1,
  "totalPages" : 1,
  "uId" : "100978"
}
```

## Topics

### Request and Response

object VppAssignmentRequest

The request for a list of assignments.

object VppAssignmentsResponse

The response that contains a list of assignments.

## See Also

### Asset and License Management

Get Assets

Get the set of assets managed by your organization.

Deprecated

Get Licenses

Get the set of licenses managed by your organization.

Deprecated

Manage Licenses

Associate and disassociate licenses with users and devices.

Deprecated

