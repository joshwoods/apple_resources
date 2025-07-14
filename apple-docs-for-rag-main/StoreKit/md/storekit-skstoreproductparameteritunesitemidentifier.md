

- StoreKit
-  SKStoreProductParameterITunesItemIdentifier 

Global Variable

# SKStoreProductParameterITunesItemIdentifier

The key representing the iTunes identifier for the item you want the store to display when the view controller is presented.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
let SKStoreProductParameterITunesItemIdentifier: String
```

## Mentioned in 

Combining parameters to generate a signature for SKAdNetwork 1

Generating the signature to validate StoreKit-rendered ads

## Discussion

The value for this key, an iTunes item identifier, is an instance of NSNumber.

To find a product’s iTunes identifier, go to linkmaker.itunes.apple.com and search for the product, then locate the iTunes identifier in the link URL. For example, the iTunes identifier for the iBooks app is 364709193.

