

- HomeKit
-  HMLocationEvent 

Class

# HMLocationEvent

An event that is evaluated based on entry to or exit from a region.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+watchOS 2.0+

``` source
class HMLocationEvent
```

## Topics

### Creating a Location Event

init(region: CLRegion)

Creates a new location event with the specified region.

### Inspecting the Region

var region: CLRegion?

The region on which events are triggered.

### Configuring the Region

func updateRegion(CLRegion, completionHandler: ((any Error)?) -> Void)

Changes the region associated with this event.

Deprecated

## Relationships

### Inherits From

- HMEvent

### Inherited By

- HMMutableLocationEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- Sendable

## See Also

### Locations

class HMMutableLocationEvent

A mutable event that is evaluated based on entry to or exit from a region.

