

- Core Media
-  CMTimeMapping 

Structure

# CMTimeMapping

A structure that maps a segment of a source time range to a target time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMTimeMapping
```

## Topics

### Creating a Timebase

init(source: CMTimeRange, target: CMTimeRange)

Creates a time mapping with a source and target time range.

init()

Creates an empty time mapping.

### Accessing Time Ranges

var source: CMTimeRange

A time range on the source timeline.

var target: CMTimeRange

A time range on the target timeline.

### Type Properties

static let invalid: CMTimeMapping

An invalid time mapping.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

