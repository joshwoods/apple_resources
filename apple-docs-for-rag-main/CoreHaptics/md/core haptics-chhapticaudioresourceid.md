

- Core Haptics
-  CHHapticAudioResourceID 

Type Alias

# CHHapticAudioResourceID

A type that identifies a custom audio resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
typealias CHHapticAudioResourceID = Int
```

## See Also

### Registering Audio Resources

func registerAudioResource(URL, options: [AnyHashable : Any]) throws -> CHHapticAudioResourceID

Registers an external audio to use as a custom waveform.

func unregisterAudioResource(CHHapticAudioResourceID) throws

Unregisters an external audio file that you previously registered with the engine.

