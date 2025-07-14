

- Audio Toolbox
-  AUEventListenerRemoveEventType(\_:\_:\_:) 

Function

# AUEventListenerRemoveEventType(\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+

``` source
func AUEventListenerRemoveEventType(
    _ inListener: AUEventListenerRef,
    _ inObject: UnsafeMutableRawPointer?,
    _ inEvent: UnsafePointer
) -> OSStatus
```

## See Also

### Responding to Events

func AUEventListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUEventListenerRef?>, Float32, Float32, dispatch_queue_t, AUEventListenerBlock) -> OSStatus

func AUEventListenerCreate(AUEventListenerProc, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, Float32, Float32, UnsafeMutablePointer&lt;AUEventListenerRef?>) -> OSStatus

func AUListenerDispose(AUParameterListenerRef) -> OSStatus

func AUEventListenerNotify(AUEventListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUEventListenerAddEventType(AUEventListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUListenerAddParameter(AUParameterListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

func AUListenerRemoveParameter(AUParameterListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

typealias AUEventListenerBlock

