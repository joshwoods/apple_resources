

- Device Management
-  Sync the List of Courses 

Web Service Endpoint

# Sync the List of Courses

Get updates about the list of courses the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/course/sync
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

## Discussion

This sync service uses a cursor returned by the full course-roster service. It returns a list of all modifications (additions or deletions) made since the cursor date, for up to 7 days.

This service may return the same course more than once. You can identify duplicates by matching their `unique_identifier` values.

## See Also

### Course Management

object BaseRosterCourse

A base course’s properties and their values.

object RosterCourse

A course’s properties and their values.

Get the List of Courses

Obtain a list of the courses the server manages.

