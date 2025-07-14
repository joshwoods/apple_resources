

- MusicKit
- MusicSubscriptionOffer
- MusicSubscriptionOffer.Options
-  init(action:messageIdentifier:itemID:affiliateToken:campaignToken:) 

Initializer

# init(action:messageIdentifier:itemID:affiliateToken:campaignToken:)

Creates options for a subscription offer sheet with specific values for common properties.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    action: MusicSubscriptionOffer.Action = .subscribe,
    messageIdentifier: MusicSubscriptionOffer.MessageIdentifier = .join,
    itemID: MusicItemID? = nil,
    affiliateToken: String? = nil,
    campaignToken: String? = nil
)
```

