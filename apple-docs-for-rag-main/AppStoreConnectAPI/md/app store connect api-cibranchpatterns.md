

- App Store Connect API
-  CiBranchPatterns 

Object

# CiBranchPatterns

Case-sensitive patterns Xcode Cloud uses to determine if a change meets branch names you configure for a workflow’s start condition.

App Store Connect API 1.5+

``` source
object CiBranchPatterns
```

## Properties

`isAllMatch`

`boolean`

​A Boolean value that indicates whether a start condition’s settings apply to all branches. If `true`, the `patterns` attribute isn’t expected. If `false`, the `patterns` attribute is required.

`patterns`

`[`CiBranchPatterns.Patterns`]`

The list of case-sensitive patterns Xcode Cloud uses to determine if a change meets branch names you configure for a workflow’s start condition.

## Topics

### Objects

object CiBranchPatterns.Patterns

A case-sensitive pattern Xcode Cloud uses to determine if a change meets branch names you configure for a workflow’s start condition.

