

- Core Animation
- CALayer
-  superlayer 

Instance Property

# superlayer

The superlayer of the layer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var superlayer: CALayer? { get }
```

## Discussion

The superlayer manages the layout of its sublayers.

## See Also

### Managing the Layer Hierarchy

var sublayers: [CALayer]?

An array containing the layer’s sublayers.

func addSublayer(CALayer)

Appends the layer to the layer’s list of sublayers.

func removeFromSuperlayer()

Detaches the layer from its parent layer.

func insertSublayer(CALayer, at: UInt32)

Inserts the specified layer into the receiver’s list of sublayers at the specified index.

func insertSublayer(CALayer, below: CALayer?)

Inserts the specified sublayer below a different sublayer that already belongs to the receiver.

func insertSublayer(CALayer, above: CALayer?)

Inserts the specified sublayer above a different sublayer that already belongs to the receiver.

func replaceSublayer(CALayer, with: CALayer)

Replaces the specified sublayer with a different layer object.

