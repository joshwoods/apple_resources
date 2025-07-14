

- TipKit
- Tips
- Tips.Event
-  sendDonation(\_:) 

Instance Method

# sendDonation(\_:)

Asynchronously donates an event with no associated `Donation` value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func sendDonation(_ completion: (() -> Void)? = nil) where DonationInfo == Tips.EmptyDonation
```

Available when `DonationInfo` conforms to `Decodable`, `Encodable`, and `Sendable`.

## Parameters 

`completion`  

Called upon completion of the event donation.

## See Also

### Add Donations

func donate() async

Donates an event with no associated `Donation` value.

func donate(DonationInfo) async

Donates an event along with its associated `Donation` value.

func sendDonation(DonationInfo, (() -> Void)?)

Asynchronously donates an event along with its associated `Donation` value.

