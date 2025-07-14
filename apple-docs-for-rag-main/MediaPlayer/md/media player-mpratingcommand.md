

- Media Player
-  MPRatingCommand 

Class

# MPRatingCommand

An object that provides a detailed rating for the playing item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPRatingCommand
```

## Topics

### Defining maximum and minimum ratings

var maximumRating: Float

The maximum rating for a command.

var minimumRating: Float

The minimum rating for a command.

## Relationships

### Inherits From

- MPRemoteCommand

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

class MPFeedbackCommandEvent

An event requesting a change in the feedback setting.

class MPRatingCommandEvent

An event requesting a change in the rating.

