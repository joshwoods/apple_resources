

- Audio Toolbox
-  AudioOutputUnitPublish(\_:\_:\_:\_:) Deprecated

Function

# AudioOutputUnitPublish(\_:\_:\_:\_:)

Registers an audio output unit for use by other applications.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioOutputUnitPublish(
    _ inDesc: UnsafePointer,
    _ inName: CFString,
    _ inVersion: UInt32,
    _ inOutputUnit: AudioUnit
) -> OSStatus
```

Deprecated

Inter-App Audio API is deprecated in favor of Audio Units

## See Also

### Inter-App Audio

func AudioOutputUnitGetHostIcon(AudioUnit, Float) -> UIImage?

The host app’s icon.

Deprecated

func AudioComponentGetIcon(AudioComponent, Float) -> UIImage?

The UIImage of the audio component’s icon.

Deprecated

func AudioComponentGetLastActiveTime(AudioComponent) -> CFAbsoluteTime

The time at which the application publishing the component was last active.

Deprecated

