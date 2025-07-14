

- DeviceActivity
- DeviceActivityFilter
-  DeviceActivityFilter.Users 

Structure

# DeviceActivityFilter.Users

A type your app uses to indicate which users to include in a device activity report.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Users
```

## Topics

### Operators

static func == (DeviceActivityFilter.Users, DeviceActivityFilter.Users) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let all: DeviceActivityFilter.Users

Filters data for all users that the current iCloud user has permission to report device activity.

static let children: DeviceActivityFilter.Users

Filters data for the children in the current user’s iCloud family.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

