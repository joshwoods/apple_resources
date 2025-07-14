

- Core Haptics
- CHHapticEngine
-  unregisterAudioResource(\_:) 

Instance Method

# unregisterAudioResource(\_:)

Unregisters an external audio file that you previously registered with the engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func unregisterAudioResource(_ resourceID: CHHapticAudioResourceID) throws
```

## Parameters 

`resourceID`  

The ID of the audio resource you’d like to unregister.

## See Also

### Registering Audio Resources

func registerAudioResource(URL, options: [AnyHashable : Any]) throws -> CHHapticAudioResourceID

Registers an external audio to use as a custom waveform.

typealias CHHapticAudioResourceID

A type that identifies a custom audio resource.

