

- App Store Connect API
-  CiTagPatterns 

Object

# CiTagPatterns

Case-sensitive patterns Xcode Cloud uses to determine if a change meets tag names you configure for a workflow’s start condition.

App Store Connect API 1.5+

``` source
object CiTagPatterns
```

## Properties

`isAllMatch`

`boolean`

​A Boolean value that indicates whether a start condition’s settings apply to all tags. If `true`, the `patterns` attribute isn’t expected. If `false`, the `patterns` attribute is required.

`patterns`

`[`CiTagPatterns.Patterns`]`

The list of case-sensitive patterns Xcode Cloud uses to determine if a change meets tag names you configure for a workflow’s start condition.

## Topics

### Objects

object CiTagPatterns.Patterns

A case-sensitive pattern Xcode Cloud uses to determine if a change meets tag names you configure for a workflow’s start condition.

