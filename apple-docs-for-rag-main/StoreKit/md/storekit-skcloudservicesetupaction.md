

- StoreKit
-  SKCloudServiceSetupAction 

Structure

# SKCloudServiceSetupAction

A string used to specify the type of setup action to offer for a cloud service.

``` source
struct SKCloudServiceSetupAction
```

## Topics

### Initializers

init(rawValue: String)

Initializes a setup action to offer for a cloud service using the specified value.

### Type Properties

static let subscribe: SKCloudServiceSetupAction

A subscribe action in a cloud service setup view, such as an offer to subscribe to Apple Music.

Deprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Indicating Setup Options

static let action: SKCloudServiceSetupOptionsKey

A key that specifies the action for a setup entry point.

Deprecated

static let iTunesItemIdentifier: SKCloudServiceSetupOptionsKey

A key that specifies the iTunes Store item that the user is trying to access through the service.

Deprecated

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

