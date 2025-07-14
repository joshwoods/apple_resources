

- UIKit
- UIImage
- UIImage.Configuration
-  withTraitCollection(\_:) 

Instance Method

# withTraitCollection(\_:)

Returns a new configuration object that merges the current traits with the traits from the specified trait collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func withTraitCollection(_ traitCollection: UITraitCollection?) -> Self
```

## Parameters 

`traitCollection`  

The traits to insert or apply to the configuration object. The trait values in this parameter take precedence over the ones in the current configuration object, unless you left the trait with an unspecified value.

## Return Value

A configuration object with the merged set of traits.

## Discussion

Use this method to augment or change the traits in the current configuration object. This method prefers the values from `traitCollection` over the values in the current configuration object. If the value of the trait is unspecified in both collections, it remains unspecified in the new collection.

## See Also

### Modifying a configuration object

func applying(UIImage.Configuration?) -> Self

Returns a configuration object that applies the specified configuration values on top of the current object’s values.

