

- Quartz
-  QCPlugInExecutionMode Deprecated

Structure

# QCPlugInExecutionMode

Execution modes for custom patches.

macOS 10.4–10.15Deprecated

``` source
struct QCPlugInExecutionMode
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Constants

var kQCPlugInExecutionModeProvider: QCPlugInExecutionMode

A provider execution mode. The custom patch executes on demand—that is, whenever data is requested of it, but at most once per frame.

var kQCPlugInExecutionModeProcessor: QCPlugInExecutionMode

A processor execution mode. The custom patch executes whenever its inputs change or if the time change (assuming it’s time-dependent).

var kQCPlugInExecutionModeConsumer: QCPlugInExecutionMode

A consumer execution mode. The custom patch always executes assuming the value of its Enable input port is `true`. (The Enable port is automatically added by the system.)

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

struct QCPlugInTimeMode

Time modes for custom patches.

Deprecated

