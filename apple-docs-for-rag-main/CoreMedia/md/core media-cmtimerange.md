

- Core Media
-  CMTimeRange 

Structure

# CMTimeRange

A structure that represents a time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMTimeRange
```

## Topics

### Creating Time Ranges

init()

Creates an empty time range at zero.

init(start: CMTime, duration: CMTime)

Creates a valid time range with a start time and duration.

init(start: CMTime, end: CMTime)

Creates a valid time range from a start and end time.

### Inspecting Time Ranges

var start: CMTime

The start time of the time range.

var end: CMTime

The end time of the time range.

var duration: CMTime

The duration of the time range.

var isValid: Bool

A Boolean value that indicates whether the time range is valid.

var isEmpty: Bool

A Boolean value that indicates whether the time range is empty.

var isIndefinite: Bool

A Boolean value that indicates whether the time range is indefinite.

### Finding Elements

func containsTime(CMTime) -> Bool

Returns a Boolean value that indicates whether the time range contains a time.

func containsTimeRange(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether the time range contains another time range.

### Combining Time Ranges

func intersection(CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements that are common to both this time range and the given time range.

func union(CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements of both this time range and the given time range.

### Constants

static let zero: CMTimeRange

A constant for generating an empty time range at zero.

static let invalid: CMTimeRange

A constant for generating an invalid time range.

### Operators

static func != (CMTimeRange, CMTimeRange) -> Bool

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

