

- AppKit
- NSScrollView
-  horizontalScrollElasticity 

Instance Property

# horizontalScrollElasticity

The scroll view’s horizontal scrolling elasticity mode.

macOS 10.7+

``` source
@MainActor
var horizontalScrollElasticity: NSScrollView.Elasticity { get set }
```

## Discussion

A scroll view can scroll its contents past its bounds to achieve an elastic effect.

When set to NSScrollView.Elasticity.automatic, scrolling the horizontal axis beyond its document bounds only occurs if the document width is greater than the view width, or the vertical scroller is hidden and the horizontal scroller is visible. The default value is NSScrollView.Elasticity.automatic.

See NSScrollView.Elasticity for possible values.

## See Also

### Specifying the Scroll View Elasticity

var verticalScrollElasticity: NSScrollView.Elasticity

The scroll view’s vertical scrolling elasticity mode.

