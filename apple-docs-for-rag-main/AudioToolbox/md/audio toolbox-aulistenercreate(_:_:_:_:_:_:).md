

- Audio Toolbox
-  AUListenerCreate(\_:\_:\_:\_:\_:\_:) 

Function

# AUListenerCreate(\_:\_:\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AUListenerCreate(
    _ inProc: AUParameterListenerProc,
    _ inUserData: UnsafeMutableRawPointer,
    _ inRunLoop: CFRunLoop?,
    _ inRunLoopMode: CFString?,
    _ inNotificationInterval: Float32,
    _ outListener: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Monitoring Parameter Changes

func AUListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUParameterListenerRef?>, Float32, dispatch_queue_t, AUParameterListenerBlock) -> OSStatus

func AUParameterListenerNotify(AUParameterListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

func AUParameterFormatValue(Float64, UnsafePointer&lt;AudioUnitParameter>, UnsafeMutablePointer&lt;CChar>, UInt32) -> UnsafeMutablePointer&lt;CChar>

func AUParameterSet(AUParameterListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>, AudioUnitParameterValue, UInt32) -> OSStatus

func AUParameterValueFromLinear(Float32, UnsafePointer&lt;AudioUnitParameter>) -> AudioUnitParameterValue

func AUParameterValueToLinear(AudioUnitParameterValue, UnsafePointer&lt;AudioUnitParameter>) -> Float32

typealias AUParameterListenerBlock

typealias AUParameterListenerProc

typealias AUParameterListenerRef

typealias AUImplementorDisplayNameWithLengthCallback

A block called to obtain a parameter node’s display name, possibly truncated to a desired length.

typealias AUImplementorStringFromValueCallback

A block called to convert a parameter value to a string representation.

typealias AUImplementorValueFromStringCallback

A block called to convert a string to a parameter value.

