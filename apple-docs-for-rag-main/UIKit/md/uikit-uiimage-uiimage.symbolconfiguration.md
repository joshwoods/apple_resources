

- UIKit
- UIImage
-  UIImage.SymbolConfiguration 

Class

# UIImage.SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class SymbolConfiguration
```

## Mentioned in 

Configuring and displaying symbol images in your UI

## Overview

Symbol image configuration objects include details such as the point size, scale, text style, weight, and font to apply to your symbol image. The system uses these details to determine which variant of the image to use and how to scale or style the image.

UIImage.SymbolConfiguration objects are immutable after you create them. If you use the applying(_:) method on the object, the new image attributes replace any previous attributes you supplied. After creating a symbol configuration object, assign it to the preferredSymbolConfiguration property of the UIImageView object you use to display the image. If you draw the image directly, use the withConfiguration(_:) method to create a new image that contains the new attributes.

## Topics

### Creating a symbol configuration

convenience init(pointSize: CGFloat)

Creates a configuration object with the specified point-size information.

convenience init(pointSize: CGFloat, weight: UIImage.SymbolWeight)

Creates a configuration object with the specified point-size and weight information.

convenience init(pointSize: CGFloat, weight: UIImage.SymbolWeight, scale: UIImage.SymbolScale)

Creates a configuration object with the specified point-size, weight, and scale information.

convenience init(scale: UIImage.SymbolScale)

Creates a configuration object with the specified scale information.

convenience init(textStyle: UIFont.TextStyle)

Creates a configuration object with the specified font text style information.

convenience init(textStyle: UIFont.TextStyle, scale: UIImage.SymbolScale)

Creates a configuration object with the specified font text style and scale information.

convenience init(weight: UIImage.SymbolWeight)

Creates a configuration object with the specified weight information.

convenience init(font: UIFont)

Creates a configuration object with the specified font information.

convenience init(font: UIFont, scale: UIImage.SymbolScale)

Creates a configuration object with the specified font and scale information.

enum SymbolScale

Constants that indicate which scale variant of a symbol image to use.

enum SymbolWeight

Constants that indicate which weight variant of a symbol image to use.

### Creating a color configuration

convenience init(hierarchicalColor: UIColor)

Creates a color configuration with a color scheme that originates from one color.

convenience init(paletteColors: [UIColor])

Creates a color configuration with a color scheme from a palette of multiple colors.

class func preferringMulticolor() -> Self

Creates a color configuration that specifies that the symbol image uses its multicolor variant, if one exists.

class func preferringMonochrome() -> Self

Creates a color configuration that specifies that the symbol image uses its monochrome variant.

### Getting an unspecified configuration

class var unspecified: UIImage.SymbolConfiguration

A symbol configuration object that contains unspecified values for all attributes.

### Removing configuration attributes

func configurationWithoutPointSizeAndWeight() -> Self

Returns a copy of the current symbol configuration object without point-size and weight information.

func configurationWithoutScale() -> Self

Returns a copy of the current symbol configuration object without scale information.

func configurationWithoutTextStyle() -> Self

Returns a copy of the current symbol configuration object without font text style information.

func configurationWithoutWeight() -> Self

Returns a copy of the current symbol configuration object without weight information.

### Comparing symbol image configurations

func isEqual(to: UIImage.SymbolConfiguration?) -> Bool

Returns a Boolean value that indicates whether the configuration objects are equivalent.

## Relationships

### Inherits From

- UIImage.Configuration

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

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

