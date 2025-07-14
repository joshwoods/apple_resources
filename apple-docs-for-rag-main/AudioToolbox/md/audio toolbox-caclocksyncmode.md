

- Audio Toolbox
-  CAClockSyncMode 

Enumeration

# CAClockSyncMode

macOS

``` source
enum CAClockSyncMode
```

## Topics

### Constants

case `internal`

case midiClockTransport

case mtcTransport

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

### Accessing Clock Properties

func CAClockGetProperty(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func CAClockGetPropertyInfo(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

func CAClockSetProperty(CAClockRef, CAClockPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

enum CAClockPropertyID

