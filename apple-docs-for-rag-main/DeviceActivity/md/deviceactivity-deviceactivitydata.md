

- DeviceActivity
-  DeviceActivityData 

Structure

# DeviceActivityData

Represents the activity of a DeviceActivityData.User on a particular DeviceActivityData.Device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct DeviceActivityData
```

## Topics

### Structures

struct ActivitySegment

Represents the user’s activity during a particular date interval.

struct ApplicationActivity

struct CategoryActivity

A categorized representation of a user’s application and web domain activity.

struct Device

A device for which to report activity data.

struct User

struct WebDomainActivity

### Operators

static func == (DeviceActivityData, DeviceActivityData) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var activitySegments: DeviceActivityResults&lt;DeviceActivityData.ActivitySegment>

The activity of the user divided into segments.

var device: DeviceActivityData.Device

The device associated with the activity report.

var hashValue: Int

The hash value.

var lastUpdatedDate: Date

The date when the system last updated the data for this device.

var segmentInterval: DeviceActivityFilter.SegmentInterval

The segment interval of each DeviceActivityData.ActivitySegment in activitySegments.

var user: DeviceActivityData.User

The user associated with the activity report.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

