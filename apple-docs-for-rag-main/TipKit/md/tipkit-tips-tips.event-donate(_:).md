

- TipKit
- Tips
- Tips.Event
-  donate(\_:) 

Instance Method

# donate(\_:)

Donates an event along with its associated `Donation` value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func donate(_ donation: DonationInfo) async
```

Available when `DonationInfo` conforms to `Decodable`, `Encodable`, and `Sendable`.

## Parameters 

`donation`  

Associated donation value.

## See Also

### Add Donations

func donate() async

Donates an event with no associated `Donation` value.

func sendDonation((() -> Void)?)

Asynchronously donates an event with no associated `Donation` value.

func sendDonation(DonationInfo, (() -> Void)?)

Asynchronously donates an event along with its associated `Donation` value.

