

- App Store Connect API
- CiBranchPatterns
-  CiBranchPatterns.Patterns 

Object

# CiBranchPatterns.Patterns

A case-sensitive pattern Xcode Cloud uses to determine if a change meets branch names you configure for a workflow’s start condition.

App Store Connect API 1.5+

``` source
object CiBranchPatterns.Patterns
```

## Properties

`isPrefix`

`boolean`

A Boolean value that indicates whether the pattern matches the start of a branch name, or the exact branch name.

`pattern`

`string`

A case-sensitive string. If the string is a prefix pattern, Xcode Cloud starts a build when the changed branch name starts with this string. Otherwise, Xcode Cloud starts a build when the changed branch name exactly matches this string.

