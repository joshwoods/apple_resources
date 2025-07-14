

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  palette(\_:) 

Type Method

# palette(\_:)

Returns a multilevel shading instance constructed from an array of shading instances.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func palette(_ array: [GraphicsContext.Shading]) -> GraphicsContext.Shading
```

## Parameters 

`array`  

An array of shading instances. The array must contain at least one element.

## Return Value

A shading instance composed from the given instances.

## See Also

### Composite shading types

static var backdrop: GraphicsContext.Shading

A shading instance that draws a copy of the current background.

