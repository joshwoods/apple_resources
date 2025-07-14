

- UIKit
-  UIFontMetrics 

Class

# UIFontMetrics

A utility object for obtaining custom fonts that scale to support Dynamic Type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class UIFontMetrics
```

## Mentioned in 

Scaling Fonts Automatically

## Overview

Use a UIFontMetrics object to support scalable custom fonts in your app. You create a font metrics object that specifies the font style—for example, body or title—that you want to use in your app. You then pass your custom font to the scaledFont(for:) method (or one of the other methods of this class) to obtain a font object that is based on your custom font, has the appropriate style information, and automatically scales to match the current Dynamic Type settings.

## Topics

### Creating a Font Metrics Object

init(forTextStyle: UIFont.TextStyle)

Creates a font metrics object for the specified text style.

class var `default`: UIFontMetrics

The default font metrics object for content.

struct TextStyle

Constants that describe the preferred styles for fonts.

### Creating Scaled Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

func scaledFont(for: UIFont) -> UIFont

Returns a version of the specified font that adopts the current font metrics.

func scaledFont(for: UIFont, compatibleWith: UITraitCollection?) -> UIFont

Returns a version of the specified font that adopts the current font metrics and supports the specified traits.

func scaledFont(for: UIFont, maximumPointSize: CGFloat) -> UIFont

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified maximum size.

func scaledFont(for: UIFont, maximumPointSize: CGFloat, compatibleWith: UITraitCollection?) -> UIFont

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified traits and size.

### Scaling Layout Values

func scaledValue(for: CGFloat) -> CGFloat

Scales an arbitrary layout value based on the current Dynamic Type settings.

func scaledValue(for: CGFloat, compatibleWith: UITraitCollection?) -> CGFloat

Scales an arbitrary layout value based on the current Dynamic Type settings and the specified traits.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Adding a Custom Font to Your App

Add a custom font to your app and use it in your app’s interface.

class UIFont

An object that provides access to the font’s characteristics.

class UIFontDescriptor

A collection of attributes that describes a font.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

