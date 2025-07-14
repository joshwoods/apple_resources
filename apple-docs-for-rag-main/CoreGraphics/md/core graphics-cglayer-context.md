

- Core Graphics
- CGLayer
-  context 

Instance Property

# context

Returns the graphics context associated with a layer object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var context: CGContext? { get }
```

## Discussion

The context that’s returned is the context for the layer itself, not the context that you specified when you created the layer.

## See Also

### Examining a Layer

var size: CGSize

Returns the width and height of a layer object.

