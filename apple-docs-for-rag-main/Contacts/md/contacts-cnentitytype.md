

- Contacts
-  CNEntityType 

Enumeration

# CNEntityType

The entities the user can grant access to.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNEntityType
```

## Topics

### Entities

case contacts

The user’s contacts.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting access to the user’s contacts

func requestAccess(for: CNEntityType, completionHandler: (Bool, (any Error)?) -> Void)

Requests access to the user’s contacts.

class func authorizationStatus(for: CNEntityType) -> CNAuthorizationStatus

Returns the current authorization status to access the contact data.

enum CNAuthorizationStatus

An authorization status the user can grant for an app to access the specified entity type.

