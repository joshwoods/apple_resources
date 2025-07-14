

- UIKit
- UIImage
- UIImage.SymbolConfiguration
-  init(scale:) 

Initializer

# init(scale:)

Creates a configuration object with the specified scale information.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(scale: UIImage.SymbolScale)
```

## Parameters 

`scale`  

The symbol image scale variant to select. Use this parameter to make the image appear bigger or smaller than surrounding content. For a list of possible values, see UIImage.SymbolScale.

## Return Value

A new symbol configuration object with the specified information.

## See Also

### Creating a symbol configuration

convenience init(pointSize: CGFloat)

Creates a configuration object with the specified point-size information.

convenience init(pointSize: CGFloat, weight: UIImage.SymbolWeight)

Creates a configuration object with the specified point-size and weight information.

convenience init(pointSize: CGFloat, weight: UIImage.SymbolWeight, scale: UIImage.SymbolScale)

Creates a configuration object with the specified point-size, weight, and scale information.

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

