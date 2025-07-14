

- Core Graphics
- CGFont
-  init(\_:) 

Initializer

# init(\_:)

Creates a font object from data supplied from a data provider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(_ provider: CGDataProvider)
```

## Parameters 

`provider`  

A data provider.

## Return Value

The font object or `NULL` if the font can’t be created. In Objective-C, you’re responsible for releasing this object using CGFontRelease.

## Discussion

Before drawing text in a Core Graphics context, you must set the font in the current graphics state by calling the function setFontSize(_:).

## See Also

### Creating Font Objects

init?(CFString)

Creates a font object corresponding to the font specified by a PostScript or full name.

