

- StoreKit
-  SKCloudServiceSetupMessageIdentifier 

Structure

# SKCloudServiceSetupMessageIdentifier

Identifiers for the available messages the setup view can present to the user.

``` source
struct SKCloudServiceSetupMessageIdentifier
```

## Topics

### Initializing Identifiers

init(rawValue: String)

Initializes a cloud service setup message identifier based on the provided raw value.

### Message Identifiers

static let addMusic: SKCloudServiceSetupMessageIdentifier

Message identifier for adding music.

Deprecated

static let connect: SKCloudServiceSetupMessageIdentifier

Message identifier for connecting.

Deprecated

static let join: SKCloudServiceSetupMessageIdentifier

Message identifier for joining.

Deprecated

static let playMusic: SKCloudServiceSetupMessageIdentifier

Message identifier for playing music.

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

