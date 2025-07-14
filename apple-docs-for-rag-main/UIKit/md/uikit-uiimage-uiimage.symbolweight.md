

- UIKit
- UIImage
-  UIImage.SymbolWeight 

Enumeration

# UIImage.SymbolWeight

Constants that indicate which weight variant of a symbol image to use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum SymbolWeight
```

## Overview

The definition of a symbol image includes multiple scale and weight variants. The weight variants offer a way to progressively thicken some or all of the image’s lines. Weights do not correspond to a specific line thickness.

## Topics

### Symbol image weights

case unspecified

An unspecified symbol image weight.

case ultraLight

An ultralight weight.

case thin

A thin weight

case light

A light weight.

case regular

A regular weight.

case medium

A medium weight.

case semibold

A semibold weight.

case bold

A bold weight.

case heavy

A heavy weight.

case black

An ultra-heavy weight.

### Getting the font weight

func fontWeight() -> UIFont.Weight

The font weight for the specified symbol weight.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

