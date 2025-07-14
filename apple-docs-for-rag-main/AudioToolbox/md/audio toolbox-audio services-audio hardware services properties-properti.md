

- Audio Toolbox
- Audio Services
-  Audio Hardware Services Properties 

API Collection

# Audio Hardware Services Properties

Property identifiers that apply to HAL audio objects only when accessed via the Audio Hardware Services.

## Topics

### Constants

var kAudioHardwareServiceProperty_ServiceRestarted: AudioObjectPropertySelector

Used, with a HAL audio object property listener callback, as a flag that indicates a hardware service restart. The property’s `Float32` value has no meaning. When the hardware service restarts, any associated application state, such as cached data or property listener callbacks, must be re-established.

var kAudioHardwareServiceDeviceProperty_VirtualMainBalance: AudioObjectPropertySelector

var kAudioHardwareServiceDeviceProperty_VirtualMainVolume: AudioObjectPropertySelector

## See Also

### Managing System Sound Services Properties

func AudioServicesGetPropertyInfo(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about a System Sound Services property.

func AudioServicesGetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Gets a specified System Sound Services property value.

func AudioServicesSetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value for a specified System Sound Services property.

typealias AudioServicesPropertyID

The data type for a system sound property identifier.

System Sound Services Property Identifiers

Property identifiers used when playing alerts with System Sound Services.

