

- Audio Toolbox
-  AUImplementorStringFromValueCallback 

Type Alias

# AUImplementorStringFromValueCallback

A block called to convert a parameter value to a string representation.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUImplementorStringFromValueCallback = (AUParameter, UnsafePointer?) -> String
```

## Discussion

This block is only of interest to audio unit subclasses.

The block returns a string representing a parameter value.

The block takes the following parameters:

param  
The parameter that contains the value.

value  
The parameter value to be converted.

## See Also

### Related Documentation

var implementorStringFromValueCallback: AUImplementorStringFromValueCallback

The callback for providing a string representation of a parameter value.

### Monitoring Parameter Changes

func AUListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUParameterListenerRef?>, Float32, dispatch_queue_t, AUParameterListenerBlock) -> OSStatus

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

typealias AUImplementorValueFromStringCallback

A block called to convert a string to a parameter value.

