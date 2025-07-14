

- Quartz
-  QCPlugInTimeMode Deprecated

Structure

# QCPlugInTimeMode

Time modes for custom patches.

macOS 10.4–10.15Deprecated

``` source
struct QCPlugInTimeMode
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Constants

var kQCPlugInTimeModeNone: QCPlugInTimeMode

No time dependency. The custom patch does not depend on time at all. (It does not use the `time` parameter of the `execute:atTime:withArguments:` method.)

var kQCPlugInTimeModeIdle: QCPlugInTimeMode

An idle time dependency. The custom patch does not depend on time but needs the system to execute it periodically. For example if the custom patch connects to a piece of hardware, to ensure that it pulls data from the hardware, you would set the custom patch time dependency to idle time mode. This time mode is typically used with providers.\]\]

var kQCPlugInTimeModeTimeBase: QCPlugInTimeMode

A time base dependency. The custom patch does depend on time explicitly and has a time base defined by the system. (It uses the `time` parameter of the `execute:atTime:withArguments:` method.)

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Structures

struct QCPlugInExecutionMode

Execution modes for custom patches.

Deprecated

