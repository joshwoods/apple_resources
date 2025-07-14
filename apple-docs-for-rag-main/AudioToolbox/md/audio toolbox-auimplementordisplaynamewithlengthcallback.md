

- Audio Toolbox
-  AUImplementorDisplayNameWithLengthCallback 

Type Alias

# AUImplementorDisplayNameWithLengthCallback

A block called to obtain a parameter node’s display name, possibly truncated to a desired length.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUImplementorDisplayNameWithLengthCallback = (AUParameterNode, Int) -> String
```

## Discussion

This block is only of interest to audio unit subclasses.

The block returns a truncated parameter node display name.

The block takes the following parameters:

node  
The parameter node to query.

desiredLength  
The desired length, in characters, of the display name.

## See Also

### Related Documentation

var implementorDisplayNameWithLengthCallback: AUImplementorDisplayNameWithLengthCallback

The callback for obtaining an abbreviated version of a parameter node display name.

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

typealias AUImplementorStringFromValueCallback

A block called to convert a parameter value to a string representation.

typealias AUImplementorValueFromStringCallback

A block called to convert a string to a parameter value.

