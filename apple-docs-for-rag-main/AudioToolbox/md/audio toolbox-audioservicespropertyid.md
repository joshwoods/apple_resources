

- Audio Toolbox
-  AudioServicesPropertyID 

Type Alias

# AudioServicesPropertyID

The data type for a system sound property identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioServicesPropertyID = UInt32
```

## Discussion

System Audio Services properties are listed in System Sound Services Property Identifiers.

## See Also

### Managing System Sound Services Properties

func AudioServicesGetPropertyInfo(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about a System Sound Services property.

func AudioServicesGetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Gets a specified System Sound Services property value.

func AudioServicesSetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value for a specified System Sound Services property.

System Sound Services Property Identifiers

Property identifiers used when playing alerts with System Sound Services.

Audio Hardware Services Properties

Property identifiers that apply to HAL audio objects only when accessed via the Audio Hardware Services.

