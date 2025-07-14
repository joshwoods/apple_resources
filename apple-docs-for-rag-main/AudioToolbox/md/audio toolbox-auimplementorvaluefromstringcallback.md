

- Audio Toolbox
-  AUImplementorValueFromStringCallback 

Type Alias

# AUImplementorValueFromStringCallback

A block called to convert a string to a parameter value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUImplementorValueFromStringCallback = (AUParameter, String) -> AUValue
```

## Discussion

This block is only of interest to audio unit subclasses.

The block returns the current value of the parameter.

The block takes the following parameters:

param  
The parameter whose value will be changed.

string  
The string that contains the new parameter value.

## See Also

### Related Documentation

var implementorValueFromStringCallback: AUImplementorValueFromStringCallback

The callback for converting a string to a parameter value.

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

typealias AUImplementorStringFromValueCallback

A block called to convert a parameter value to a string representation.

