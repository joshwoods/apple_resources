

- StoreKit
- SKStoreProductViewController
-  loadProduct(parameters:impression:) 

Instance Method

# loadProduct(parameters:impression:)

AdAttributionKitStoreKitiOS 17.4+iPadOS 17.4+

``` source
@MainActor @preconcurrency
func loadProduct(
    parameters: [String : Any],
    impression: AppImpression
) async throws
```

## See Also

### Loading a new product screen

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

func loadProduct(withParameters: [String : Any], completionBlock: ((Bool, (any Error)?) -> Void)?)

Loads a new product screen to display.

func loadProduct(withParameters: [String : Any], impression: SKAdImpression, completionBlock: ((Bool, (any Error)?) -> Void)?)

func loadProduct(parameters: [String : Any], impression: AppImpression, reengagementURL: URL) async throws

Product Dictionary Keys

Keys for identifying products and the tokens for affiliates and campaigns.

