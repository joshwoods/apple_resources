

- Core Graphics
- CGContext
-  beginTransparencyLayer(in:auxiliaryInfo:) 

Instance Method

# beginTransparencyLayer(in:auxiliaryInfo:)

Begins a transparency layer whose contents are bounded by the specified rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func beginTransparencyLayer(
    in rect: CGRect,
    auxiliaryInfo auxInfo: CFDictionary?
)
```

## Parameters 

`rect`  

The rectangle, specified in user space, that bounds the transparency layer.

`auxInfo`  

A dictionary that specifies any additional information, or `nil`.

## Discussion

This function is identical to beginTransparencyLayer(auxiliaryInfo:) except that the content of the transparency layer is within the bounds of the provided rectangle.

## See Also

### Working with Transparency Layers

func beginTransparencyLayer(auxiliaryInfo: CFDictionary?)

Begins a transparency layer.

func endTransparencyLayer()

Ends a transparency layer.

