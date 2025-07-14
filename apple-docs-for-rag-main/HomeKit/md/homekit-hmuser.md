

- HomeKit
-  HMUser 

Class

# HMUser

A person in the home who may have access to control accessories and services in the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMUser
```

## Topics

### Getting Information About the User

var name: String

The name of the user.

var uniqueIdentifier: UUID

A unique identifier for the user.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing users

func manageUsers(completionHandler: ((any Error)?) -> Void)

Presents a view controller to manage users of the home.

var currentUser: HMUser

The current HomeKit user.

