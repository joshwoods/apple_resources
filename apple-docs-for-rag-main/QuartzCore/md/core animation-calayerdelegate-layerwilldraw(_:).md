

- Core Animation
- CALayerDelegate
-  layerWillDraw(\_:) 

Instance Method

# layerWillDraw(\_:)

Notifies the delegate of an imminent draw.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func layerWillDraw(_ layer: CALayer)
```

## Parameters 

`layer`  

The layer whose contents will be drawn.

## Discussion

The layerWillDraw(_:) method is called before draw(_:in:). You can use this method to configure any layer state affecting contents prior to draw(_:in:) such as contentsFormat and isOpaque.

Important

This method is not called if the delegate implements display(_:).

## See Also

### Providing the Layer’s Content

func display(CALayer)

Tells the delegate to implement the display process.

func draw(CALayer, in: CGContext)

Tells the delegate to implement the display process using the layer’s context.

