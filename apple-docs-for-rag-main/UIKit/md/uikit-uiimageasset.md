

- UIKit
-  UIImageAsset 

Class

# UIImageAsset

A container for a collection of images that represent multiple ways of describing a single piece of artwork.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class UIImageAsset
```

## Overview

A common use case for UIImageAsset is the grouping of multiple images of the same item at different display scales. Image asset objects aren’t assigned to instances of UIImage rather; UIImage provides an asset when multiple representations of an image are available. Images retrieved from image asset catalogs using the init(named:) or init(named:in:compatibleWith:) methods automatically have an image asset object that allows access to other images from the catalog.

### Register an image

When you register an image with an image asset, you associate a UITraitCollection object with the image. The trait collection must contain the displayScale and userInterfaceIdiom trait properties. If you don’t define these traits in the trait collection, the following defaults are assigned:

- displayScale = `1.0`

- userInterfaceIdiom = UIUserInterfaceIdiom.unspecified

For example, if you create a trait collection that only contains a horizontal size class, the default display scale and idiom are added when the image is registered.

### Retrieve an image

When you retrieve or unregister an image from an image asset, you do so using the trait collection that was used to register the image. To ensure the correct image is retrieved, the trait collection used must contain the displayScale and userInterfaceIdiom traits. If these traits aren’t defined in the trait collection, the following defaults are assigned:

- displayScale = scale of the current device

- userInterfaceIdiom = the type of interface used on the current device

For example, if you create a trait collection that only contains a horizontal size class, the default display scale and idiom of the current device are added when searching the `UIImageAsset` for an image.

UIImageView automatically retrieves the correct image when traitCollectionDidChange(_:) is called on it.

## Topics

### Initializing an image asset

init()

Creates a new image asset object.

init?(coder: NSCoder)

Creates an image asset from data in an unarchiver.

### Registering and unregistering images

func register(UIImage, with: UITraitCollection)

Registers an image with the specified trait collection.

func register(UIImage, with: UIImage.Configuration)

Registers an image with the specified image configuration details.

func unregister(imageWith: UITraitCollection)

Unregisters the image with the specified trait collection from the image asset.

func unregisterImage(with: UIImage.Configuration)

Unregisters the image with the specified image configuration details from the image asset.

### Retrieving an image from an image asset

func image(with: UITraitCollection) -> UIImage

Retrieves the variant of the image that best matches the specified trait collection.

func image(with: UIImage.Configuration) -> UIImage

Retrieves the variant of the image that best matches the specified image configuration details.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Assets

class NSDataAsset

An object from a data set type stored in an asset catalog.

