

- UIKit
- UITraitCollection
-  containsTraits(in:) Deprecated

Instance Method

# containsTraits(in:)

Queries whether a trait collection contains all of another trait collection’s values.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
func containsTraits(in trait: UITraitCollection?) -> Bool
```

## Parameters 

`trait`  

A trait collection that you want to compare to the current trait collection.

## Return Value

This method returns true if the receiver contains all of the trait values in the trait collection passed in the `trait` parameter, and returns false otherwise.

## Discussion

Use this method to compare two standalone trait collections, or to compare the iOS interface environment’s trait collection to a standalone trait collection.

## See Also

### Comparing trait collections

func hasDifferentColorAppearance(comparedTo: UITraitCollection?) -> Bool

Queries whether changing between the specified and current trait collections would affect color values.

