

- UIKit
- UIImage
-  configuration 

Instance Property

# configuration

The configuration details for the image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var configuration: UIImage.Configuration? { get }
```

## Discussion

Use this property to access the traits associated with the image. The system uses the specified traits to determine which variant of the image to load and draw, falling back on the current environment for any unspecified traits. The default value of this property is a configuration object with unspecified traits.

You can’t modify this property directly, but you can use the withConfiguration(_:) method to create a new image object with a specific set of traits. You might do so when you want to render the image yourself using a specific set of traits.

If the image is a symbol image, this property always contains a UIImage.SymbolConfiguration object.

## See Also

### Getting the image configuration

var symbolConfiguration: UIImage.SymbolConfiguration?

The configuration details for a symbol image.

var traitCollection: UITraitCollection

The trait collection that describes the current variant of the image.

