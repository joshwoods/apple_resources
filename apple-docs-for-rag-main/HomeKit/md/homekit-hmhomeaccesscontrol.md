

- HomeKit
-  HMHomeAccessControl 

Class

# HMHomeAccessControl

The access privileges of a user associated with a home.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMHomeAccessControl
```

## Topics

### Getting the Privileges of a User

var isAdministrator: Bool

Specifies if the user has administrative privileges for the home.

## Relationships

### Inherits From

- HMAccessControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Controlling user access

func homeAccessControl(for: HMUser) -> HMHomeAccessControl

Retrieves the access level of a user associated with the home.

class HMAccessControl

An abstract superclass for accessing user privileges.

let HMUserFailedAccessoriesKey: String

The key for retrieving details of what accessories failed to add or remove a user.

