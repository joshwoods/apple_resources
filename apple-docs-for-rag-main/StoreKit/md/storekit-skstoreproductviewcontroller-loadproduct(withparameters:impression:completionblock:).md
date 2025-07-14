

- StoreKit
- SKStoreProductViewController
-  loadProduct(withParameters:impression:completionBlock:) 

Instance Method

# loadProduct(withParameters:impression:completionBlock:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor
func loadProduct(
    withParameters parameters: [String : Any],
    impression: SKAdImpression,
    completionBlock block: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func loadProduct(
    withParameters parameters: [String : Any],
    impression: SKAdImpression
) async throws -> Bool
```

## See Also

### Loading a new product screen

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

func loadProduct(withParameters: [String : Any], completionBlock: ((Bool, (any Error)?) -> Void)?)

Loads a new product screen to display.

func loadProduct(parameters: [String : Any], impression: AppImpression) async throws

func loadProduct(parameters: [String : Any], impression: AppImpression, reengagementURL: URL) async throws

Product Dictionary Keys

Keys for identifying products and the tokens for affiliates and campaigns.

