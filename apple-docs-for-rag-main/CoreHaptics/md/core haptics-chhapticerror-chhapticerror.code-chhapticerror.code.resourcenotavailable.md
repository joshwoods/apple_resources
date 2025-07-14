

- Core Haptics
- CHHapticError
- CHHapticError.Code
-  CHHapticError.Code.resourceNotAvailable 

Case

# CHHapticError.Code.resourceNotAvailable

The requested operation couldn’t finish due to a limit on available resources.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
case resourceNotAvailable
```

## Discussion

This error occurs when your app’s registered audio resources reach the limit. The app needs to unregister others to make resources available again.

## See Also

### Error Codes

case badEventEntry

An event is missing a required field.

case badParameterEntry

A parameter in an event is missing a required field.

case engineNotRunning

Your app requested haptic playback when the engine wasn’t running.

case engineStartTimeout

The haptic engine timed out while starting.

case fileNotFound

The system couldn’t find an audio file or haptic asset.

case insufficientPower

The operation failed due to power restrictions.

case invalidAudioResource

A pattern dictionary or an event array contain a reference to an invalid audio resource.

case invalidAudioSession

The system invalidated the audio session associated with the haptic engine.

case invalidEngineParameter

Your app attempted to initialize the haptic engine with an invalid configuration parameter.

case invalidEventDuration

An event in the dictionary has an invalid duration.

case invalidEventTime

The time of an event in the dictionary is invalid.

case invalidEventType

The type of an event in the dictionary is invalid.

case invalidParameterType

A pattern dictionary or parameter array contains an unknown or invalid parameter type.

case invalidPatternData

Your app passed an invalid pattern to the haptic engine or player.

case invalidPatternDictionary

A pattern in the dictionary is missing a required field.

