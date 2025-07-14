

- Audio Toolbox
-  kAudioHardwareServiceDeviceProperty_VirtualMainVolume 

Global Variable

# kAudioHardwareServiceDeviceProperty_VirtualMainVolume

macOS

``` source
var kAudioHardwareServiceDeviceProperty_VirtualMainVolume: AudioObjectPropertySelector { get }
```

## See Also

### Constants

var kAudioHardwareServiceProperty_ServiceRestarted: AudioObjectPropertySelector

Used, with a HAL audio object property listener callback, as a flag that indicates a hardware service restart. The property’s `Float32` value has no meaning. When the hardware service restarts, any associated application state, such as cached data or property listener callbacks, must be re-established.

var kAudioHardwareServiceDeviceProperty_VirtualMainBalance: AudioObjectPropertySelector

