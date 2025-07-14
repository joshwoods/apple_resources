

- StoreKit
- SKCloudServiceSetupOptionsKey
-  messageIdentifier Deprecated

Type Property

# messageIdentifier

A key that is used to select the main message presented to the user for this setup view.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
static let messageIdentifier: SKCloudServiceSetupOptionsKey
```

Deprecated

Use the messageIdentifier property of MusicSubscriptionOffer.Options from MusicKit

## Mentioned in 

Offering Apple Music Subscription in Your App

## Discussion

If this key is missing, the setup view is configured as if it is using the join key by default.

## See Also

### Indicating Setup Options

static let action: SKCloudServiceSetupOptionsKey

A key that specifies the action for a setup entry point.

Deprecated

struct SKCloudServiceSetupAction

A string used to specify the type of setup action to offer for a cloud service.

static let iTunesItemIdentifier: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store item that the user is trying to access through the service.

Deprecated

static let affiliateToken: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store affiliate token.

Deprecated

static let campaignToken: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store affiliate campaign token.

Deprecated

struct SKCloudServiceSetupMessageIdentifier

Identifiers for the available messages the setup view can present to the user.

