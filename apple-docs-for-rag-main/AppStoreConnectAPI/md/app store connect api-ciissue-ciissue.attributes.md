

- App Store Connect API
- CiIssue
-  CiIssue.Attributes 

Object

# CiIssue.Attributes

The attributes that describe an Issues resource.

App Store Connect API 1.5+

``` source
object CiIssue.Attributes
```

## Properties

`category`

`string`

​A string representing the issue’s category; for example, the name of the build phase where the issue occurred.

`fileSource`

FileLocation

The file and line number where Xcode Cloud encountered an issue.

`issueType`

`string`

A string that indicates what kind of issue Xcode Cloud encountered.

Possible Values: `ANALYZER_WARNING, ERROR, TEST_FAILURE, WARNING`

`message`

`string`

Information about the issue that occurred.

