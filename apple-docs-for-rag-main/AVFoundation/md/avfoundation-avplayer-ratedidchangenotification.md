

- AVFoundation
- AVPlayer
-  rateDidChangeNotification 

Type Property

# rateDidChangeNotification

A notification that a player posts when its rate changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class let rateDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

Observing this notification is similar to key-value observing the rate property, except the notification provides additional information about the rate change in the user information dictionary.

## Topics

### User Information Keys

class let rateDidChangeOriginatingParticipantKey: String

A key to retrieve the identifier of the participant that originates the rate change.

class let rateDidChangeReasonKey: String

A key to retrieve the reason for the rate change.

struct RateDidChangeReason

A structure that represents a rate change reason.

## See Also

### Controlling Playback

var defaultRate: Float

A default rate at which to begin playback.

func play()

Begins playback of the current item.

func pause()

Pauses playback of the current item.

var rate: Float

The current playback rate.

