

- AVFoundation
- AVPlayer
-  rateDidChangeOriginatingParticipantKey 

Type Property

# rateDidChangeOriginatingParticipantKey

A key to retrieve the identifier of the participant that originates the rate change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class let rateDidChangeOriginatingParticipantKey: String
```

## Discussion

The associated value is a UUID of a participant in the playback coordinator’s otherParticipants array.

## See Also

### User Information Keys

class let rateDidChangeReasonKey: String

A key to retrieve the reason for the rate change.

struct RateDidChangeReason

A structure that represents a rate change reason.

