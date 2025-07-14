

- App Store Connect API
- CiBuildAction
-  CiBuildAction.Attributes 

Object

# CiBuildAction.Attributes

The attributes that describe a Build Actions resource.

App Store Connect API 1.5+

``` source
object CiBuildAction.Attributes
```

## Properties

`actionType`

CiActionType

The type of the build action.

`completionStatus`

CiCompletionStatus

The status of the action.

`executionProgress`

CiExecutionProgress

A string that indicates the progress of the build action.

`finishedDate`

`date-time`

The date and time when Xcode Cloud finished performing the action.

`isRequiredToPass`

`boolean`

A Boolean value that indicates whether the action must succeed in order for a build to succeed.

`issueCounts`

CiIssueCounts

An integer value that represents the number of issues Xcode Cloud encountered when it performed the action.

`name`

`string`

The name of the build action; for example, `Archive iOS`.

`startedDate`

`date-time`

The date and time when Xcode Cloud started performing the action.

## Topics

### Types

type CiActionType

A string that represents the type of an Xcode Cloud workflow’s action.

## See Also

### Objects

object CiBuildAction.Relationships

The relationships of the Build Actions resource you included in the request and those on which you can operate.

