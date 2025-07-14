

- Audio Toolbox
-  CAClockGetProperty(\_:\_:\_:\_:) 

Function

# CAClockGetProperty(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockGetProperty(
    _ inCAClock: CAClockRef,
    _ inPropertyID: CAClockPropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Accessing Clock Properties

func CAClockGetPropertyInfo(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

func CAClockSetProperty(CAClockRef, CAClockPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

enum CAClockPropertyID

enum CAClockSyncMode

