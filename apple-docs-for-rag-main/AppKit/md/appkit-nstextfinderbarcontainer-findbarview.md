

- AppKit
- NSTextFinderBarContainer
-  findBarView 

Instance Property

# findBarView

The view assigned by the text bar as the find bar view for the container.

macOS

``` source
var findBarView: NSView? { get set }
```

**Required**

## Discussion

This property is managed by `NSTextFinder` and you must not set this property.

The container may freely modify the view’s width, but should not modify its height.

## See Also

### Find Bar View

func contentView() -> NSView?

A view hierarchy that contains all the views which display the contents being searched.

var isFindBarVisible: Bool

Returns whether the container should display its find bar.

**Required**

