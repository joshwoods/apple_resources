

- Core Graphics
- CGFont
-  init(\_:) 

Initializer

# init(\_:)

Creates a font object corresponding to the font specified by a PostScript or full name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(_ name: CFString)
```

## Parameters 

`name`  

The PostScript or full name of a font.

## Return Value

The font object or `NULL` if the font can’t be created. In Objective-C, you’re responsible for releasing this object using CGFontRelease.

## Discussion

Before drawing text in a Core Graphics context, you must set the font in the current graphics state by calling the function setFont(_:).

## See Also

### Creating Font Objects

init?(CGDataProvider)

Creates a font object from data supplied from a data provider.

