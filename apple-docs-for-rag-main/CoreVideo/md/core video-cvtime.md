

- Core Video
-  CVTime 

Structure

# CVTime

A structure for reporting Core Video time values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVTime
```

## Overview

This structure is equivalent to the QuickTime `QTTime` structure.

## Topics

### Initializers

init()

init(timeValue: Int64, timeScale: Int32, flags: Int32)

### Properties

var flags: Int32

The flags associated with the `CVTime` value. See CVTime Values for possible values. If `kCVTimeIsIndefinite` is set, you should not use any of the other fields in this structure.

var timeScale: Int32

The time scale for this value.

var timeValue: Int64

The time value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

CVTimeStamp

A structure for representing a display timestamp.

struct CVSMPTETime

A structure for holding an SMPTE time.

