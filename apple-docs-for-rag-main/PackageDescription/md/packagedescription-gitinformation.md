

- PackageDescription
-  GitInformation 

Structure

# GitInformation

Information about the git status of a given package, if available.

SwiftPM 6.0+

``` source
struct GitInformation
```

## Topics

### Instance Properties

let currentCommit: String

The commit currently checked out.

let currentTag: String?

The version tag currently checked out, if available.

let hasUncommittedChanges: Bool

Whether or not there are uncommitted changes in the current repository.

## Relationships

### Conforms To

- Sendable

