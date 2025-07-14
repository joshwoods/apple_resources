

- TipKit
- Tips
- Tips.Event
-  sendDonation(\_:\_:) 

Instance Method

# sendDonation(\_:\_:)

Asynchronously donates an event along with its associated `Donation` value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func sendDonation(
    _ donation: DonationInfo,
    _ completion: (() -> Void)? = nil
)
```

Available when `DonationInfo` conforms to `Decodable`, `Encodable`, and `Sendable`.

## Parameters 

`donation`  

Associated donation value.

`completion`  

Called upon completion of the event donation.

## See Also

### Add Donations

func donate() async

Donates an event with no associated `Donation` value.

func donate(DonationInfo) async

Donates an event along with its associated `Donation` value.

func sendDonation((() -> Void)?)

Asynchronously donates an event with no associated `Donation` value.

