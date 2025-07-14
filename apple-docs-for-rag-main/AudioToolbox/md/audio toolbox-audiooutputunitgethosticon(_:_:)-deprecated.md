

- Audio Toolbox
-  AudioOutputUnitGetHostIcon(\_:\_:) Deprecated

Function

# AudioOutputUnitGetHostIcon(\_:\_:)

The host app’s icon.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioOutputUnitGetHostIcon(
    _ au: AudioUnit,
    _ desiredPointSize: Float
) -> UIImage?
```

Deprecated

Inter-App Audio API is deprecated in favor of Audio Units

## Discussion

The UIImage of the host app’s icon.

## See Also

### Inter-App Audio

func AudioOutputUnitPublish(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioUnit) -> OSStatus

Registers an audio output unit for use by other applications.

Deprecated

func AudioComponentGetIcon(AudioComponent, Float) -> UIImage?

The UIImage of the audio component’s icon.

Deprecated

func AudioComponentGetLastActiveTime(AudioComponent) -> CFAbsoluteTime

The time at which the application publishing the component was last active.

Deprecated

