

- Audio Toolbox
-  AudioComponentGetIcon(\_:\_:) Deprecated

Function

# AudioComponentGetIcon(\_:\_:)

The UIImage of the audio component’s icon.

iOS 7.0–14.0DeprecatediPadOS 7.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 10.11–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

**macOS**

``` source
func AudioComponentGetIcon(_ comp: AudioComponent) -> NSImage?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func AudioComponentGetIcon(
    _ comp: AudioComponent,
    _ desiredPointSize: Float
) -> UIImage?
```

## See Also

### Inter-App Audio

func AudioOutputUnitPublish(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioUnit) -> OSStatus

Registers an audio output unit for use by other applications.

Deprecated

func AudioOutputUnitGetHostIcon(AudioUnit, Float) -> UIImage?

The host app’s icon.

Deprecated

func AudioComponentGetLastActiveTime(AudioComponent) -> CFAbsoluteTime

The time at which the application publishing the component was last active.

Deprecated

