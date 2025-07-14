

- StoreKit
-  SKCloudServiceSetupOptionsKey 

Structure

# SKCloudServiceSetupOptionsKey

Keys to specify the types of setup options for a cloud service.

``` source
struct SKCloudServiceSetupOptionsKey
```

## Topics

### Initializing

init(rawValue: String)

Initializes a cloud service setup options key based on the provided raw value.

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

static let messageIdentifier: SKCloudServiceSetupOptionsKey

A key that is used to select the main message presented to the user for this setup view.

Deprecated

struct SKCloudServiceSetupMessageIdentifier

Identifiers for the available messages the setup view can present to the user.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Loading the setup view

Offering Apple Music Subscription in Your App

Allow eligible customers to subscribe to Apple Music.

func load(options: [SKCloudServiceSetupOptionsKey : Any], completionHandler: ((Bool, (any Error)?) -> Void)?)

Loads the cloud service setup view with the specified options.

Deprecated

class SKArcadeService

