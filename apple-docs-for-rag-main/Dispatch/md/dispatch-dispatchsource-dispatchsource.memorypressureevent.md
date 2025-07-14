

- Dispatch
- DispatchSource
-  DispatchSource.MemoryPressureEvent 

Structure

# DispatchSource.MemoryPressureEvent

Memory pressure events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MemoryPressureEvent
```

## Topics

### Memory Pressure Event Flags

static let all: DispatchSource.MemoryPressureEvent

All memory pressure events.

static let normal: DispatchSource.MemoryPressureEvent

An event indicating that the system memory pressure condition changed to normal.

static let warning: DispatchSource.MemoryPressureEvent

An event indicating that the system memory pressure condition changed to warning.

static let critical: DispatchSource.MemoryPressureEvent

An event indicating that the system memory pressure condition changed to critical.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a Memory Pressure Source

class func makeMemoryPressureSource(eventMask: DispatchSource.MemoryPressureEvent, queue: DispatchQueue?) -> any DispatchSourceMemoryPressure

Creates a new dispatch source object that monitors the system for changes in the memory pressure condition.

protocol DispatchSourceMemoryPressure

A dispatch source that monitors the system for changes in the memory pressure condition.

