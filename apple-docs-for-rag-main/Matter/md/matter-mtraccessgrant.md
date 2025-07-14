

- Matter
-  MTRAccessGrant 

Class

# MTRAccessGrant

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRAccessGrant
```

## Topics

### Initializers

init(forAllNodesWith: MTRAccessControlEntryPrivilege)

init?(forCASEAuthenticatedTag: NSNumber, privilege: MTRAccessControlEntryPrivilege)

init?(forGroupID: NSNumber, privilege: MTRAccessControlEntryPrivilege)

init?(forNodeID: NSNumber, privilege: MTRAccessControlEntryPrivilege)

### Instance Properties

var authenticationMode: MTRAccessControlEntryAuthMode

var grantedPrivilege: MTRAccessControlEntryPrivilege

var subjectID: NSNumber?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

