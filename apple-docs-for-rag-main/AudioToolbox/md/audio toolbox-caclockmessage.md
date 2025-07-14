

- Audio Toolbox
-  CAClockMessage 

Enumeration

# CAClockMessage

macOS

``` source
enum CAClockMessage
```

## Topics

### Constants

case armed

case disarmed

case propertyChanged

case startTimeSet

case started

case stopped

case wrongSMPTEFormat

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Adding and Removing Listeners

func CAClockAddListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

func CAClockRemoveListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

typealias CAClockListenerProc

