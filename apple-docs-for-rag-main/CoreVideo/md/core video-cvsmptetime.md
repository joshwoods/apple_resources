

- Core Video
-  CVSMPTETime 

Structure

# CVSMPTETime

A structure for holding an SMPTE time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVSMPTETime
```

## Topics

### Initializers

init()

init(subframes: Int16, subframeDivisor: Int16, counter: UInt32, type: UInt32, flags: UInt32, hours: Int16, minutes: Int16, seconds: Int16, frames: Int16)

### Properties

var counter: UInt32

The total number of messages received.

var flags: UInt32

A set of flags that indicate the SMPTE state.

var frames: Int16

The number of frames in the full message.

var hours: Int16

The number of hours in the full message.

var minutes: Int16

The number of minutes in the full message.

var seconds: Int16

The number of seconds in the full message.

var subframeDivisor: Int16

The number of subframes per frame (typically, 80).

var subframes: Int16

The number of subframes in the full message.

var type: UInt32

The kind of SMPTE time type.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CVTime

A structure for reporting Core Video time values.

CVTimeStamp

A structure for representing a display timestamp.

