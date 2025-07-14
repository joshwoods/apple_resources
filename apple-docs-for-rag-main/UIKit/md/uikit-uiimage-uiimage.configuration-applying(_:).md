

- UIKit
- UIImage
- UIImage.Configuration
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns a configuration object that applies the specified configuration values on top of the current object’s values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func applying(_ otherConfiguration: UIImage.Configuration?) -> Self
```

## Parameters 

`otherConfiguration`  

The configuration attributes to apply over the current attributes. Values in this object take precedence over values in the image’s current configuration object.

## Return Value

A configuration object with the specified image configuration attributes and merged traits.

## Mentioned in 

Configuring and displaying symbol images in your UI

## Discussion

This method merges the traits from `otherConfiguration` with the current object’s trait collection, giving precedence to traits in `otherConfiguration` unless the trait is unspecified. For image-specific traits, this method replaces the current image attributes with the attributes in `otherConfiguration`.

## See Also

### Modifying a configuration object

func withTraitCollection(UITraitCollection?) -> Self

Returns a new configuration object that merges the current traits with the traits from the specified trait collection.

