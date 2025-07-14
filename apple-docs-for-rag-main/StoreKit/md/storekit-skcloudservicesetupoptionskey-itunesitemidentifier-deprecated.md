

- StoreKit
- SKCloudServiceSetupOptionsKey
-  iTunesItemIdentifier Deprecated

Type Property

# iTunesItemIdentifier

A key that specifies the iTunes Store item that the user is trying to access through the service.

iOS 10.1–18.0DeprecatediPadOS 10.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedtvOS 10.0–18.0Deprecated

``` source
static let iTunesItemIdentifier: SKCloudServiceSetupOptionsKey
```

Deprecated

Use the itemID property of MusicSubscriptionOffer.Options from MusicKit

## Discussion

The only iTunes Store items that are supported are song, video, playlist, and album.

## See Also

### Indicating Setup Options

static let action: SKCloudServiceSetupOptionsKey

A key that specifies the action for a setup entry point.

Deprecated

struct SKCloudServiceSetupAction

A string used to specify the type of setup action to offer for a cloud service.

static let affiliateToken: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store affiliate token.

Deprecated

static let campaignToken: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store affiliate campaign token.

Deprecated

static let messageIdentifier: SKCloudServiceSetupOptionsKey

A key that is used to select the main message presented to the user for this setup view.

Deprecated

struct SKCloudServiceSetupMessageIdentifier

Identifiers for the available messages the setup view can present to the user.

