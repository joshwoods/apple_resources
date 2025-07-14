

- AVFAudio
-  AVAudioUnitComponentManager 

Class

# AVAudioUnitComponentManager

An object that provides a way to search and query audio components that the system registers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitComponentManager
```

## Overview

The component manager has methods to find various information about the audio components without opening them. Currently, you can only search audio components that are audio units.

The class supports system tags and arbitrary user tags. You can tag each audio unit as part of its definition. Audio unit hosts, such as Logic or GarageBand, can present groupings of audio units according to the tags.

You can search for audio units in the following ways:

- Using a `NSPredicate` instance that contains search strings for tags or descriptions

- Using a block to match on a custom criteria

- Using an `AudioComponentDescription`

## Topics

### Getting the unit audio component manager

class func shared() -> Self

Gets the shared component manager instance.

### Getting matching audio components

func components(matching: AudioComponentDescription) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the description.

func components(matching: NSPredicate) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the search predicate.

func components(passingTest: (AVAudioUnitComponent, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [AVAudioUnitComponent]

Gets an array of audio components that pass the block method.

### Getting audio unit tags

var standardLocalizedTagNames: [String]

An array of the localized standard system tags the audio units define.

var tagNames: [String]

An array of all tags the audio unit associates with the current user, and the system tags the audio units define.

### Observing registration changes

class let registrationsChangedNotification: NSNotification.Name

A notification the component manager generates when it updates its list of components.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Component management

class AVAudioUnitComponent

An object that provides details about an audio unit.

