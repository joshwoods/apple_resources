

- Core Animation
- CALayer
-  scroll(\_:) 

Instance Method

# scroll(\_:)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified point lies at the origin of the scroll layer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func scroll(_ p: CGPoint)
```

## Parameters 

`p`  

The point in the current layer that should be scrolled into position.

## Discussion

If the layer is not contained by a CAScrollLayer object, this method does nothing.

## See Also

### Scrolling

var visibleRect: CGRect

The visible region of the layer in its own coordinate space.

func scrollRectToVisible(CGRect)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified rectangle becomes visible.

