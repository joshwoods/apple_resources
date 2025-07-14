

- CarPlay
-  CPVoiceControlState 

Class

# CPVoiceControlState

A voice control state containing title variants and images for use by a voice control template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPVoiceControlState
```

## Topics

### Creating a Voice Control State

init(identifier: String, titleVariants: [String]?, image: UIImage?, repeats: Bool)

Creates a voice control state.

### Getting State Information

var identifier: String

The string that your app uses to identify the voice control state.

var titleVariants: [String]?

The array of title variants for the voice control state.

var image: UIImage?

The image displayed while the voice control template is in this state.

var repeats: Bool

A Boolean value that indicates whether the display of an animated image repeats the animation sequence indefinitely.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating a Voice Control Template

init(voiceControlStates: [CPVoiceControlState])

Creates a voice control template with a list of voice control states.

