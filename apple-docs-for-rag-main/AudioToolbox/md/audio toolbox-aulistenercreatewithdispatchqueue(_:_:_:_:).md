

- Audio Toolbox
-  AUListenerCreateWithDispatchQueue(\_:\_:\_:\_:) 

Function

# AUListenerCreateWithDispatchQueue(\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AUListenerCreateWithDispatchQueue(
    _ outListener: UnsafeMutablePointer,
    _ inNotificationInterval: Float32,
    _ inDispatchQueue: dispatch_queue_t,
    _ inBlock: @escaping AUParameterListenerBlock
) -> OSStatus
```

## See Also

### Monitoring Parameter Changes

func AUListenerCreate(AUParameterListenerProc, UnsafeMutableRawPointer, CFRunLoop?, CFString?, Float32, UnsafeMutablePointer&lt;AUParameterListenerRef?>) -> OSStatus

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

