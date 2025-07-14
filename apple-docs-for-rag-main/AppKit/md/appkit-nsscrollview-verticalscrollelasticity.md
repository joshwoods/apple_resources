

- AppKit
- NSScrollView
-  verticalScrollElasticity 

Instance Property

# verticalScrollElasticity

The scroll view’s vertical scrolling elasticity mode.

macOS 10.7+

``` source
@MainActor
var verticalScrollElasticity: NSScrollView.Elasticity { get set }
```

## Discussion

A scroll view can scroll its contents past its bounds to achieve an elastic effect.

When set to NSScrollView.Elasticity.automatic, scrolling the vertical axis beyond its document bounds only occurs if any of the following are true: the vertical scroller is visible, the content height is greater than view height, or the horizontal scroller hidden. The default value is NSScrollView.Elasticity.automatic.

See NSScrollView.Elasticity for possible values.

## See Also

### Specifying the Scroll View Elasticity

var horizontalScrollElasticity: NSScrollView.Elasticity

The scroll view’s horizontal scrolling elasticity mode.

