

- Core Animation
- CALayer
-  sublayers 

Instance Property

# sublayers

An array containing the layer’s sublayers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var sublayers: [CALayer]? { get set }
```

## Discussion

The sublayers are listed in back to front order. The default value of this property is `nil`.

### Special Considerations

When setting the sublayers property to an array populated with layer objects, each layer in the array must not already have a superlayer—that is, its superlayer property must currently be `nil`.

## See Also

### Managing the Layer Hierarchy

var superlayer: CALayer?

The superlayer of the layer.

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

