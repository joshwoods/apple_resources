

- Core Haptics
- CHHapticError
-  resourceNotAvailable 

Type Property

# resourceNotAvailable

The framework didn’t locate a named resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static var resourceNotAvailable: CHHapticError.Code { get }
```

## Discussion

This error occurs when you specify an invalid audio file path.

## See Also

### Error Code Constants

static var badEventEntry: CHHapticError.Code

An event is missing a required field.

static var badParameterEntry: CHHapticError.Code

A parameter in an event is missing a required field.

static var engineNotRunning: CHHapticError.Code

Your app requested haptic playback when the engine wasn’t running.

static var engineStartTimeout: CHHapticError.Code

The haptic engine timed out while starting.

static var fileNotFound: CHHapticError.Code

The system couldn’t find an audio file or haptic asset.

static var insufficientPower: CHHapticError.Code

The operation failed due to power restrictions.

static var invalidAudioResource: CHHapticError.Code

A pattern dictionary or an event array contain a reference to an invalid audio resource.

static var invalidAudioSession: CHHapticError.Code

The system invalidated the audio session associated with the haptic engine.

static var invalidEngineParameter: CHHapticError.Code

Your app attempted to initialize the haptic engine with an invalid configuration parameter.

static var invalidEventDuration: CHHapticError.Code

An event in the dictionary has an invalid duration.

static var invalidEventTime: CHHapticError.Code

The time of an event in the dictionary is invalid.

static var invalidEventType: CHHapticError.Code

The type of an event in the dictionary is invalid.

static var invalidParameterType: CHHapticError.Code

A pattern dictionary or parameter array contains an unknown or invalid parameter type.

static var invalidPatternData: CHHapticError.Code

Your app passed an invalid pattern to the haptic engine or player.

static var invalidPatternDictionary: CHHapticError.Code

A pattern in the dictionary is missing a required field.

