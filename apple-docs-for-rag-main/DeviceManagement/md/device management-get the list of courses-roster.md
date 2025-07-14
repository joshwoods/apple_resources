

- Device Management
-  Get the List of Courses 

Web Service Endpoint

# Get the List of Courses

Obtain a list of the courses the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/course
```

## HTTP Body

RosterRequest

The object containing the request information.

Content-Type: application/json

## Response Codes

` 200 ``OK`

RosterCourseResponse

`OK`

The request was successful. The server returns a list of courses.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server was unable to process the request.

## Topics

### Response

object RosterCourseResponse

The response that contains a list of courses.

## See Also

### Course Management

object BaseRosterCourse

A base course’s properties and their values.

object RosterCourse

A course’s properties and their values.

Sync the List of Courses

Get updates about the list of courses the server manages.

