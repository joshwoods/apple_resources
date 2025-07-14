

- Audio Toolbox
-  AudioComponentGetLastActiveTime(\_:) Deprecated

Function

# AudioComponentGetLastActiveTime(\_:)

The time at which the application publishing the component was last active.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioComponentGetLastActiveTime(_ comp: AudioComponent) -> CFAbsoluteTime
```

Deprecated

Inter-App Audio API is deprecated in favor of Audio Units

## See Also

### Inter-App Audio

func AudioOutputUnitPublish(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioUnit) -> OSStatus

Registers an audio output unit for use by other applications.

Deprecated

func AudioOutputUnitGetHostIcon(AudioUnit, Float) -> UIImage?

The host app’s icon.

Deprecated

func AudioComponentGetIcon(AudioComponent, Float) -> UIImage?

The UIImage of the audio component’s icon.

Deprecated

