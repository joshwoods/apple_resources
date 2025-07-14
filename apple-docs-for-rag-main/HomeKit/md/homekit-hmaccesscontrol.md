

- HomeKit
-  HMAccessControl 

Class

# HMAccessControl

An abstract superclass for accessing user privileges.

iOS 11.2+iPadOS 11.2+Mac Catalyst 11.2+tvOS 11.2+visionOS 1.0+watchOS 4.2+

``` source
class HMAccessControl
```

## Overview

Use a concrete subclass, like HMHomeAccessControl, instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMHomeAccessControl

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

class HMHomeAccessControl

The access privileges of a user associated with a home.

let HMUserFailedAccessoriesKey: String

The key for retrieving details of what accessories failed to add or remove a user.

