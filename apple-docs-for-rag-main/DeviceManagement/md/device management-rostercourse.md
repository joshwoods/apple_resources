

- Device Management
-  RosterCourse 

Object

# RosterCourse

A course’s properties and their values.

Device Assignment ServicesVPP License Management

``` source
object RosterCourse
```

## Properties

`course_number`

`string`

The number of the course.

`name`

`string`

The course name. Maximum length 1024 UTF-8 characters.

`source`

`string`

The data source where the class was created.

Possible Values: `LDAP, SIS, CSV, MANUAL, SYSTEM, ENROLLMENT, DEP, FORMULA_GENERATED, SFTP`

`source_system_identifier`

`string`

The identifier configured by organization for the course. Maximum length is 256 UTF-8 characters. Value can be null.

`unique_identifier`

`string`

The unique identifier for the course. Maximum length 256 UTF-8 characters.

`op_date`

`string`

The time stamp, in iSO 8601 format, when the course was added, updated, or deleted.

`status`

`string`

The status for the course.

## See Also

### Course Management

object BaseRosterCourse

A base course’s properties and their values.

Get the List of Courses

Obtain a list of the courses the server manages.

Sync the List of Courses

Get updates about the list of courses the server manages.

