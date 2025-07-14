

- Core Animation
- CALayer
-  addSublayer(\_:) 

Instance Method

# addSublayer(\_:)

Appends the layer to the layer’s list of sublayers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func addSublayer(_ layer: CALayer)
```

## Parameters 

`layer`  

The layer to be added.

## Discussion

If the array in the sublayers property is `nil`, calling this method creates an array for that property and adds the specified layer to it.

## See Also

### Managing the Layer Hierarchy

var sublayers: [CALayer]?

An array containing the layer’s sublayers.

var superlayer: CALayer?

The superlayer of the layer.

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

