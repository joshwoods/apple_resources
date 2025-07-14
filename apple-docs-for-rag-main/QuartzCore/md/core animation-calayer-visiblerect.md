

- Core Animation
- CALayer
-  visibleRect 

Instance Property

# visibleRect

The visible region of the layer in its own coordinate space.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var visibleRect: CGRect { get }
```

## Discussion

The visible region is the area not clipped by the containing scroll layer.

## See Also

### Scrolling

func scroll(CGPoint)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified point lies at the origin of the scroll layer.

func scrollRectToVisible(CGRect)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified rectangle becomes visible.

