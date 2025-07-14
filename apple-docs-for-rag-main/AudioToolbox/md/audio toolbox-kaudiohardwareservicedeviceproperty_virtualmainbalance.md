

- Audio Toolbox
-  kAudioHardwareServiceDeviceProperty_VirtualMainBalance 

Global Variable

# kAudioHardwareServiceDeviceProperty_VirtualMainBalance

macOS

``` source
var kAudioHardwareServiceDeviceProperty_VirtualMainBalance: AudioObjectPropertySelector { get }
```

## See Also

### Constants

var kAudioHardwareServiceProperty_ServiceRestarted: AudioObjectPropertySelector

Used, with a HAL audio object property listener callback, as a flag that indicates a hardware service restart. The property’s `Float32` value has no meaning. When the hardware service restarts, any associated application state, such as cached data or property listener callbacks, must be re-established.

var kAudioHardwareServiceDeviceProperty_VirtualMainVolume: AudioObjectPropertySelector

