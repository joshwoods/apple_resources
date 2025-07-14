

- Core Animation
- CALayer
-  insertSublayer(\_:above:) 

Instance Method

# insertSublayer(\_:above:)

Inserts the specified sublayer above a different sublayer that already belongs to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func insertSublayer(
    _ layer: CALayer,
    above sibling: CALayer?
)
```

## Parameters 

`layer`  

The sublayer to be inserted into the current layer.

`sibling`  

An existing sublayer in the current layer. The layer in `aLayer` is inserted after this layer in the sublayers array, and thus appears in front of it visually.

## Discussion

If `sublayer` is not in the receiver’s sublayers array, this method raises an exception.

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

func insertSublayer(CALayer, at: UInt32)

Inserts the specified layer into the receiver’s list of sublayers at the specified index.

func insertSublayer(CALayer, below: CALayer?)

Inserts the specified sublayer below a different sublayer that already belongs to the receiver.

func replaceSublayer(CALayer, with: CALayer)

Replaces the specified sublayer with a different layer object.

