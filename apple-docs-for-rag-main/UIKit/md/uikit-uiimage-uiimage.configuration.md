

- UIKit
- UIImage
-  UIImage.Configuration 

Class

# UIImage.Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Configuration
```

## Overview

Images may contain multiple variants to account for environmental factors, such as whether the interface is light or dark. The image configuration object lets you override the current environment and render an image with specific attributes. For example, you might want to render a specific version of your image to your interface.

UIImage.Configuration objects are immutable and you don’t create them directly. Instead, get an existing image configuration object from a UITraitCollection or UIImage object. To add attributes to your configuration object, use the applying(_:) method to create a new object that merges the existing object’s values with new values you supply. Assign the new object to the preferredSymbolConfiguration property of the UIImageView object you use to display the image. If you draw the image directly, use the withConfiguration(_:) method to create a new image that contains the new attributes.

## Topics

### Modifying a configuration object

func applying(UIImage.Configuration?) -> Self

Returns a configuration object that applies the specified configuration values on top of the current object’s values.

func withTraitCollection(UITraitCollection?) -> Self

Returns a new configuration object that merges the current traits with the traits from the specified trait collection.

### Getting the configuration traits

var traitCollection: UITraitCollection?

The traits associated with the image configuration.

### Initializers

convenience init(locale: Locale?)

convenience init(traitCollection: UITraitCollection?)

### Instance Properties

var locale: Locale?

### Instance Methods

func withLocale(Locale?) -> Self

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIImage.SymbolConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Representations

class UIImage

An object that manages image data in your app.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

