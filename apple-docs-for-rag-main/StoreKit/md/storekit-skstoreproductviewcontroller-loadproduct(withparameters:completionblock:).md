

- StoreKit
- SKStoreProductViewController
-  loadProduct(withParameters:completionBlock:) 

Instance Method

# loadProduct(withParameters:completionBlock:)

Loads a new product screen to display.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
@MainActor
func loadProduct(
    withParameters parameters: [String : Any],
    completionBlock block: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func loadProduct(withParameters parameters: [String : Any]) async throws -> Bool
```

## Parameters 

`parameters`  

A dictionary describing the content you want the view controller to display. See Product Dictionary Keys for keys that describe the product. See Ad network install-validation keys for keys that describe an impression in an advertising campaign.

`block`  

A block to be called when the product information has been loaded from the App Store. The completion block is called on the main thread and receives the following parameters:

`result`  
true if the product information was successfully loaded, otherwise false.

`error`  
If an error occurred, this object describes the error. If the product information was successfully loaded, this value is `nil`.

## Mentioned in 

Generating the signature to validate StoreKit-rendered ads

Signing and providing ads

## Discussion

For a seamless user experience, load the product information before presenting the SKStoreProductViewController view controller. However, if you load the product information while presenting the view controller, once loaded, the product data replaces the contents of the view controller.

## See Also

### Loading a new product screen

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

func loadProduct(withParameters: [String : Any], impression: SKAdImpression, completionBlock: ((Bool, (any Error)?) -> Void)?)

func loadProduct(parameters: [String : Any], impression: AppImpression) async throws

func loadProduct(parameters: [String : Any], impression: AppImpression, reengagementURL: URL) async throws

Product Dictionary Keys

Keys for identifying products and the tokens for affiliates and campaigns.

