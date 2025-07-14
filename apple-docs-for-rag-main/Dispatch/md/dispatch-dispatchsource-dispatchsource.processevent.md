

- Dispatch
- DispatchSource
-  DispatchSource.ProcessEvent 

Structure

# DispatchSource.ProcessEvent

Events related to a process.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct ProcessEvent
```

## Topics

### Process Event Flags

static let all: DispatchSource.ProcessEvent

All process-related events.

static let exec: DispatchSource.ProcessEvent

The process became another executable image.

static let exit: DispatchSource.ProcessEvent

The process has exited (perhaps cleanly, perhaps not).

static let fork: DispatchSource.ProcessEvent

The process created one or more child processes.

static let signal: DispatchSource.ProcessEvent

The process received a UNIX signal.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a Process Source

class func makeProcessSource(identifier: pid_t, eventMask: DispatchSource.ProcessEvent, queue: DispatchQueue?) -> any DispatchSourceProcess

Creates a new dispatch source object for monitoring the specified process.

protocol DispatchSourceProcess

A dispatch source that monitors an external process for events.

