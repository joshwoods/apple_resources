

- Core Animation
- CAEmitterCell
-  contents 

Instance Property

# contents

An object that provides the contents of the layer. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var contents: Any? { get set }
```

## Discussion

A layer can set this property to a CGImage to display the image as its contents.

The default value of this property is `nil`.

## See Also

### Providing Emitter Cell Content

var contentsRect: CGRect

A rectangle (in the unit coordinate space) that specifies the portion of contents that the receiver should draw. Animatable.

var emitterCells: [CAEmitterCell]?

An optional array containing the sub-cells of this cell.

