

- Media Player
-  MPFeedbackCommandEvent 

Class

# MPFeedbackCommandEvent

An event requesting a change in the feedback setting.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPFeedbackCommandEvent
```

## Topics

### Determining the type of feedback action

var isNegative: Bool

A Boolean value that indicates whether an app should perform a negative command appropriate to the target.

## Relationships

### Inherits From

- MPRemoteCommandEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to feedback and rating events

class MPFeedbackCommand

An object that reflects the feedback state for the playing item.

class MPRatingCommand

An object that provides a detailed rating for the playing item.

class MPRatingCommandEvent

An event requesting a change in the rating.

