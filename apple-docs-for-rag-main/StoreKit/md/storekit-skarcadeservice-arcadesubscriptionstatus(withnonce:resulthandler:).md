

- StoreKit
- SKArcadeService
-  arcadeSubscriptionStatus(withNonce:resultHandler:) 

Type Method

# arcadeSubscriptionStatus(withNonce:resultHandler:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func arcadeSubscriptionStatus(
    withNonce nonce: UInt64,
    resultHandler: @escaping (Data?, UInt32, Data?, UInt32, (any Error)?) -> Void
)
```

