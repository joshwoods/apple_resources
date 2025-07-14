

- Audio Toolbox
-  kAudioHardwareServiceProperty_ServiceRestarted 

Global Variable

# kAudioHardwareServiceProperty_ServiceRestarted

Used, with a HAL audio object property listener callback, as a flag that indicates a hardware service restart. The property’s `Float32` value has no meaning. When the hardware service restarts, any associated application state, such as cached data or property listener callbacks, must be re-established.

macOS

``` source
var kAudioHardwareServiceProperty_ServiceRestarted: AudioObjectPropertySelector { get }
```

## See Also

### Constants

var kAudioHardwareServiceDeviceProperty_VirtualMainBalance: AudioObjectPropertySelector

var kAudioHardwareServiceDeviceProperty_VirtualMainVolume: AudioObjectPropertySelector

