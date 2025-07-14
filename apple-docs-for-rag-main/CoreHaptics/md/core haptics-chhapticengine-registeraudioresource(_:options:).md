

- Core Haptics
- CHHapticEngine
-  registerAudioResource(\_:options:) 

Instance Method

# registerAudioResource(\_:options:)

Registers an external audio to use as a custom waveform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func registerAudioResource(
    _ resourceURL: URL,
    options: [AnyHashable : Any] = [:]
) throws -> CHHapticAudioResourceID
```

## Parameters 

`resourceURL`  

A URL that identifies the location of the audio file to register.

`options`  

A dictionary with audio resource keys and values that describe how to play this resource.

## Return Value

An identifier for the audio resource.

## Mentioned in 

Preparing your app to play haptics

## Discussion

Before you initialize a Core Haptics event with your own audio file, use this method to register the file with the engine. Reference external audio files using a URL.

Input the value that this method returns when creating the dictionary or event representation of a haptic pattern.

Note

In an Apple Haptics and Audio File (AHAP), you specify audio files by their path, as opposed to their registered resource URL. For more information, see Representing haptic patterns in AHAP files.

## Topics

### Audio Resource Keys

let CHHapticAudioResourceKeyLoopEnabled: String

A key for a Boolean value that indicates whether to loop audio playback.

let CHHapticAudioResourceKeyUseVolumeEnvelope: String

A key for a Boolean value that indicates whether audio file playback fades in and out using an envelope.

typealias CHHapticAudioResourceKey

A type alias for a key that identifies the playback behavior of an audio resource.

## See Also

### Registering Audio Resources

func unregisterAudioResource(CHHapticAudioResourceID) throws

Unregisters an external audio file that you previously registered with the engine.

typealias CHHapticAudioResourceID

A type that identifies a custom audio resource.

