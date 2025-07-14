

- UIKit
- UIImage
-  UIImage.SymbolScale 

Enumeration

# UIImage.SymbolScale

Constants that indicate which scale variant of a symbol image to use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum SymbolScale
```

## Mentioned in 

Configuring and displaying symbol images in your UI

## Overview

The definition of a symbol image includes multiple scale and weight variants. Scale variants offer a way to define the size of the image relative to layout guides in the symbol image’s definition file. The system chooses the appropriate size variant based on the available space and configuration options.

## Topics

### Symbol image scales

case `default`

The default scale variant that matches the system usage.

case unspecified

An unspecified scale.

case small

The small variant of the symbol image.

case medium

The medium variant of the symbol image

case large

The large variant of the symbol image.

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

enum SymbolWeight

Constants that indicate which weight variant of a symbol image to use.

