

- Core Animation
- CALayer
-  removeFromSuperlayer() 

Instance Method

# removeFromSuperlayer()

Detaches the layer from its parent layer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func removeFromSuperlayer()
```

## Discussion

You can use this method to remove a layer (and all of its sublayers) from a layer hierarchy. This method updates both the superlayer’s list of sublayers and sets this layer’s superlayer property to `nil`.

## See Also

### Managing the Layer Hierarchy

var sublayers: [CALayer]?

An array containing the layer’s sublayers.

var superlayer: CALayer?

The superlayer of the layer.

func addSublayer(CALayer)

Appends the layer to the layer’s list of sublayers.

func insertSublayer(CALayer, at: UInt32)

Inserts the specified layer into the receiver’s list of sublayers at the specified index.

func insertSublayer(CALayer, below: CALayer?)

Inserts the specified sublayer below a different sublayer that already belongs to the receiver.

func insertSublayer(CALayer, above: CALayer?)

Inserts the specified sublayer above a different sublayer that already belongs to the receiver.

func replaceSublayer(CALayer, with: CALayer)

Replaces the specified sublayer with a different layer object.

