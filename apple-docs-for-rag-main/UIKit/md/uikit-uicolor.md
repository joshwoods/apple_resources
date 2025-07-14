

- UIKit
-  UIColor 

Class

# UIColor

An object that stores color data and sometimes opacity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class UIColor
```

## Mentioned in 

Customizing drawings

Determining color values with color spaces

Understanding a drag item as a promise

## Overview

Use color to customize your app’s appearance, communicate status, and help people visualize data. To learn more about using color in your apps, see Human Interface Guidelines.

UIColor provides a list of class properties that create adaptable and fixed colors such as blue, green, purple, and more. UIColor also offers properties to specify system-provided colors for UI elements such as labels, text, and buttons. You can create color objects by specifying color component values such as RGB, hue, and saturation. You can also create colors from other color objects and even create a pattern-based color from an image.

Important

Most developers have no need to subclass UIColor. The only time subclassing might be necessary is if you require support for additional color spaces or color models. If you do subclass, the properties and methods you add must be safe to use from multiple threads.

## Topics

### Getting existing colors

UI element colors

Choose colors for UI elements such as labels, text, backgrounds, and links.

Standard colors

Define standard color objects for specific shades, such as red, blue, green, black, white, and more.

Color creation

Load colors from asset catalogs and create colors from raw component values.

### Applying the color to the drawing environment

Customizing drawings

Create custom colors and patterns for drawing in your app.

func set()

Sets the color of subsequent stroke and fill operations to the color that the receiver represents.

func setFill()

Sets the color of subsequent fill operations to the color that the receiver represents.

func setStroke()

Sets the color of subsequent stroke operations to the color that the receiver represents.

### Getting the color information

Determining color values with color spaces

Change the system’s interpretation of a color value for display by selecting a color space.

var cgColor: CGColor

The Quartz color that corresponds to the color object.

var ciColor: CIColor

The Core Image color that corresponds to the color object.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the HSB color space.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the RGB color space.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the grayscale components of the color.

var accessibilityName: String

A localized description of the color for accessibility attributes.

### Resolving a dynamically generated color

func resolvedColor(with: UITraitCollection) -> UIColor

Returns the version of the current color that results from the specified traits.

### Working with color prominence

var prominence: UIColor.Prominence

func withProminence(UIColor.Prominence) -> UIColor

Returns the version of the current color that results from applying the specified prominence.

enum Prominence

A type that indicates the prominence of a color in the interface.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- NSSecureCoding
- Sendable

