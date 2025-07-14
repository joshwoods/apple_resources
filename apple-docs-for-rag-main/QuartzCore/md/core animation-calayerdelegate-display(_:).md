

- Core Animation
- CALayerDelegate
-  display(\_:) 

Instance Method

# display(\_:)

Tells the delegate to implement the display process.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func display(_ layer: CALayer)
```

## Parameters 

`layer`  

The layer whose contents need updating.

## Discussion

The display(_:) delegate method is called when the layer is marked for its content to be reloaded, typically initiated by the setNeedsDisplay() method. The typical technique for updating is to set the layer’s `contents` property.

The following code shows how you can create a class named `LayerDelegate` that implements CALayerDelegate and sets it as a layer’s (named `sublayer`) delegate. When setNeedsDisplay() is called on `sublayer`, the delegate’s display(_:) replaces its contents with a specified image.

```
let delegate = LayerDelegate()

lazy var sublayer: CALayer = {
    let layer = CALayer()

    layer.delegate = self.delegate

    return layer
}()

// When `sublayer.setNeedsDisplay()` is called, `sublayer.contents` are updated.

class LayerDelegate: NSObject, CALayerDelegate {
    func display(_ layer: CALayer) {
        layer.contents = UIImage(named: "rabbit.png")?.cgImage
    }
}
```

## See Also

### Providing the Layer’s Content

func draw(CALayer, in: CGContext)

Tells the delegate to implement the display process using the layer’s context.

func layerWillDraw(CALayer)

Notifies the delegate of an imminent draw.

