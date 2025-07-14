

- AppKit
- NSTextFinder
-  findIndicatorNeedsUpdate 

Instance Property

# findIndicatorNeedsUpdate

Invoke to specify that the find indicator needs updating when not contained within a scroll view.

macOS 10.7+

``` source
var findIndicatorNeedsUpdate: Bool { get set }
```

## Discussion

If the client object’s document is not scrolled by an instance of `NSScrollView`, then set this property to true when scrolling occurs to cause the find indicator to be updated appropriately.

