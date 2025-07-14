

- AVFoundation
- AVPlayer
-  AVPlayer.RateDidChangeReason 

Structure

# AVPlayer.RateDidChangeReason

A structure that represents a rate change reason.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct RateDidChangeReason
```

## Topics

### Initializers

init(rawValue: String)

Creates a reason with a string value.

### Rate Change Reasons

static let appBackgrounded: AVPlayer.RateDidChangeReason

An app transitions to the background.

static let audioSessionInterrupted: AVPlayer.RateDidChangeReason

The system interrupts the app’s audio session.

static let setRateCalled: AVPlayer.RateDidChangeReason

An app makes a call to set the player’s rate.

static let setRateFailed: AVPlayer.RateDidChangeReason

An attempt to change the player’s rate fails.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### User Information Keys

class let rateDidChangeOriginatingParticipantKey: String

A key to retrieve the identifier of the participant that originates the rate change.

class let rateDidChangeReasonKey: String

A key to retrieve the reason for the rate change.

