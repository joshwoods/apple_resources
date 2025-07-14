

- HealthKit
-  HKActivityMoveModeObject 

Class

# HKActivityMoveModeObject

An object that contains a movement mode value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class HKActivityMoveModeObject
```

## Topics

### Accessing the data

var activityMoveMode: HKActivityMoveMode

A property that contains the movement mode value.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Activity rings

class HKActivitySummary

An object that contains the move, exercise, and stand data for a given day.

struct HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKActivityRingView

A view that uses the Move, Exercise, and Stand activity rings to display data from a HealthKit activity summary object.

