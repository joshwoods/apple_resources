

- UIKit
- UITraitCollection
-  hasDifferentColorAppearance(comparedTo:) 

Instance Method

# hasDifferentColorAppearance(comparedTo:)

Queries whether changing between the specified and current trait collections would affect color values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func hasDifferentColorAppearance(comparedTo traitCollection: UITraitCollection?) -> Bool
```

## Parameters 

`traitCollection`  

A trait collection that you want to compare to the current trait collection.

## Return Value

true if the colors in the two trait collections differ, or false if they have the same component values.

## Discussion

Use this method to determine whether changing the traits of the current environment would also change the colors in your interface. For example, changing the userInterfaceStyle or accessibilityContrast property usually changes the colors of your interface.

## See Also

### Comparing trait collections

func containsTraits(in: UITraitCollection?) -> Bool

Queries whether a trait collection contains all of another trait collection’s values.

Deprecated

