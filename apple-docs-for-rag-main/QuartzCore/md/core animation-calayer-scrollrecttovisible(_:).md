

- Core Animation
- CALayer
-  scrollRectToVisible(\_:) 

Instance Method

# scrollRectToVisible(\_:)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified rectangle becomes visible.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func scrollRectToVisible(_ r: CGRect)
```

## Parameters 

`r`  

The rectangle to be made visible.

## Discussion

If the layer is not contained by a CAScrollLayer object, this method does nothing.

## See Also

### Scrolling

var visibleRect: CGRect

The visible region of the layer in its own coordinate space.

func scroll(CGPoint)

Initiates a scroll in the layer’s closest ancestor scroll layer so that the specified point lies at the origin of the scroll layer.

