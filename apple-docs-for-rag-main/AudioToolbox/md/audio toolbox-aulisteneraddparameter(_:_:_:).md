

- Audio Toolbox
-  AUListenerAddParameter(\_:\_:\_:) 

Function

# AUListenerAddParameter(\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AUListenerAddParameter(
    _ inListener: AUParameterListenerRef,
    _ inObject: UnsafeMutableRawPointer?,
    _ inParameter: UnsafePointer
) -> OSStatus
```

## See Also

### Responding to Events

func AUEventListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUEventListenerRef?>, Float32, Float32, dispatch_queue_t, AUEventListenerBlock) -> OSStatus

func AUEventListenerCreate(AUEventListenerProc, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, Float32, Float32, UnsafeMutablePointer&lt;AUEventListenerRef?>) -> OSStatus

func AUListenerDispose(AUParameterListenerRef) -> OSStatus

func AUEventListenerNotify(AUEventListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUEventListenerAddEventType(AUEventListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUEventListenerRemoveEventType(AUEventListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUListenerRemoveParameter(AUParameterListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

typealias AUEventListenerBlock

