

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  style(\_:) 

Type Method

# style(\_:)

Returns a shading instance that fills with the given shape style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func style(_ style: S) -> GraphicsContext.Shading where S : ShapeStyle
```

## Parameters 

`style`  

A ShapeStyle instance to draw with.

## Return Value

A shading instance filled with a shape style.

## Discussion

Styles with geometry defined in a unit coordinate space map that space to the rectangle associated with the drawn object. You can adjust that using the in(_:) method. The shape style might affect the blend mode and opacity of the drawn object.

## See Also

### Other shape styles

static var foreground: GraphicsContext.Shading

A shading instance that fills with the foreground style from the graphics context’s environment.

