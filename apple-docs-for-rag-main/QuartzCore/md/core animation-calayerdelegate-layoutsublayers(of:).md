

- Core Animation
- CALayerDelegate
-  layoutSublayers(of:) 

Instance Method

# layoutSublayers(of:)

Tells the delegate a layer’s bounds have changed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func layoutSublayers(of layer: CALayer)
```

## Parameters 

`layer`  

The layer that requires layout of its sublayers.

## Discussion

The layoutSublayers(of:) method is called when a layer’s bounds have changed and its sublayers may need rearranging, for example by changing its frame’s size. You can implement this method if you need precise control over the layout of your layer’s sublayers.

The following code shows how you can create a class named `LayerDelegate` that implements `CALayerDelegate` and sets it as a layer’s (named `sublayer`) delegate. When the layer’s size changes, the delegate’s layoutSublayers(of:) iterates over all of the sublayers of `sublayer` and resizes them to fit within it.

```
let delegate = LayerDelegate()

lazy var sublayer: CALayer = {
    let layer = CALayer()

    layer.addSublayer(CALayer())
    layer.sublayers?.first?.backgroundColor = UIColor.blue.cgColor

    layer.delegate = self.delegate

    return layer
}()

// sublayer.frame = CGRect(x: 0, y: 0, width: 510, height: 510)

class LayerDelegate: NSObject, CALayerDelegate {
    func layoutSublayers(of layer: CALayer) {
        layer.sublayers?.forEach {
            $0.frame = layer.bounds
        }
    }
}
```

