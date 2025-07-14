

- StoreKit
-  SKArcadeService 

Class

# SKArcadeService

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class SKArcadeService
```

## Topics

### Type Methods

class func arcadeSubscriptionStatus(withNonce: UInt64, resultHandler: (Data?, UInt32, Data?, UInt32, (any Error)?) -> Void)

class func registerArcadeAppWithRandom(fromLib: Data, randomFromLibLength: UInt32, resultHandler: (Data?, UInt32, Data?, UInt32, (any Error)?) -> Void)

class func repairArcadeApp()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Loading the setup view

Offering Apple Music Subscription in Your App

Allow eligible customers to subscribe to Apple Music.

struct SKCloudServiceSetupOptionsKey

Keys to specify the types of setup options for a cloud service.

func load(options: [SKCloudServiceSetupOptionsKey : Any], completionHandler: ((Bool, (any Error)?) -> Void)?)

Loads the cloud service setup view with the specified options.

Deprecated

