

- Audio Toolbox
-  CAClockSetProperty(\_:\_:\_:\_:) 

Function

# CAClockSetProperty(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockSetProperty(
    _ inCAClock: CAClockRef,
    _ inPropertyID: CAClockPropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## See Also

### Accessing Clock Properties

func CAClockGetProperty(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func CAClockGetPropertyInfo(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

enum CAClockPropertyID

enum CAClockSyncMode

