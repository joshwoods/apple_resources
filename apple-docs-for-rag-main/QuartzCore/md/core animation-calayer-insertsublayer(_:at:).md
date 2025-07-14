

- Core Animation
- CALayer
-  insertSublayer(\_:at:) 

Instance Method

# insertSublayer(\_:at:)

Inserts the specified layer into the receiver’s list of sublayers at the specified index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func insertSublayer(
    _ layer: CALayer,
    at idx: UInt32
)
```

## Parameters 

`layer`  

The sublayer to be inserted into the current layer.

`idx`  

The index at which to insert `aLayer`. This value must be a valid 0-based index into the sublayers array.

## See Also

### Managing the Layer Hierarchy

var sublayers: [CALayer]?

An array containing the layer’s sublayers.

var superlayer: CALayer?

The superlayer of the layer.

func addSublayer(CALayer)

Appends the layer to the layer’s list of sublayers.

func removeFromSuperlayer()

Detaches the layer from its parent layer.

func insertSublayer(CALayer, below: CALayer?)

Inserts the specified sublayer below a different sublayer that already belongs to the receiver.

func insertSublayer(CALayer, above: CALayer?)

Inserts the specified sublayer above a different sublayer that already belongs to the receiver.

func replaceSublayer(CALayer, with: CALayer)

Replaces the specified sublayer with a different layer object.

