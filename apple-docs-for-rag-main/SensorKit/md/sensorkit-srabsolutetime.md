

- SensorKit
-  SRAbsoluteTime 

Structure

# SRAbsoluteTime

A value that describes when the system records the data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct SRAbsoluteTime
```

## Discussion

This value tracks monotonically increasing device-specific time, unlike mach_continuous_time, which keeps tracking across reboots.

Although a fetch can query a device other than a phone (such as a paired watch), the framework consistently describes time according to the phone. Any fetch results from a paired watch are in the phone’s version of SRAbsoluteTime.

## Topics

### Creating an Absolute Time

init(CFTimeInterval)

Creates an absolute time from a raw value.

init(rawValue: CFTimeInterval)

Creates an absolute time from a raw value.

### Accessing the Current Absolute Time

static func current() -> SRAbsoluteTime

Provides the current absolute time.

### Converting Absolute Times

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining the Time Range

var from: SRAbsoluteTime

Fetches sample information that occurs after this time.

var to: SRAbsoluteTime

Fetches sample information that occurs before this time.

static func current() -> SRAbsoluteTime

Provides the current absolute time.

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

