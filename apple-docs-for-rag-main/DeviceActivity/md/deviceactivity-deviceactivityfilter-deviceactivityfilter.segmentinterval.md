

- DeviceActivity
- DeviceActivityFilter
-  DeviceActivityFilter.SegmentInterval 

Enumeration

# DeviceActivityFilter.SegmentInterval

A type indicating the interval at which the system subdivides device activity data within a specified date interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum SegmentInterval
```

## Topics

### Operators

static func == (DeviceActivityFilter.SegmentInterval, DeviceActivityFilter.SegmentInterval) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case daily(during: DateInterval)

Indicates that the system aggregates data into daily segments within the specified interval.

case hourly(during: DateInterval)

Indicates that the system aggregates data into hourly segments within the specified interval.

case weekly(during: DateInterval)

Indicates that the system aggregates data into weekly segments within the specified interval.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

