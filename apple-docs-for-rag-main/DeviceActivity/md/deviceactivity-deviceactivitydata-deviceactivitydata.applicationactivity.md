

- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.ApplicationActivity 

Structure

# DeviceActivityData.ApplicationActivity

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct ApplicationActivity
```

## Topics

### Operators

static func == (DeviceActivityData.ApplicationActivity, DeviceActivityData.ApplicationActivity) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var application: Application

The application that accumulated the activity.

var hashValue: Int

The hash value.

var numberOfNotifications: Int

The number of notifications made by the application.

var numberOfPickups: Int

The number of pickups made directly to the application.

var totalActivityDuration: TimeInterval

The total activity for this application.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

