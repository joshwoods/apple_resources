

- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.User 

Structure

# DeviceActivityData.User

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct User
```

## Topics

### Operators

static func == (DeviceActivityData.User, DeviceActivityData.User) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var appleID: String?

The AppleID of the user.

var hashValue: Int

The hash value.

var nameComponents: PersonNameComponents?

The user’s name.

var role: DeviceActivityData.User.FamilyRole

The type of the user.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum FamilyRole

A type describing the user’s role in their iCloud family.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

