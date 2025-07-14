

- Core Animation
- CALayer
-  replaceSublayer(\_:with:) 

Instance Method

# replaceSublayer(\_:with:)

Replaces the specified sublayer with a different layer object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func replaceSublayer(
    _ oldLayer: CALayer,
    with newLayer: CALayer
)
```

## Parameters 

`oldLayer`  

The layer to be replaced.

`newLayer`  

The layer with which to replace `oldLayer`.

## Discussion

If `oldLayer` is not in the receiver’s sublayers array, the behavior of this method is undefined.

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

func insertSublayer(CALayer, above: CALayer?)

Inserts the specified sublayer above a different sublayer that already belongs to the receiver.

