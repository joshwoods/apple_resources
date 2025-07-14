

- AppKit
- NSTextFinderBarContainer
-  contentView() 

Instance Method

# contentView()

A view hierarchy that contains all the views which display the contents being searched.

macOS

``` source
optional func contentView() -> NSView?
```

## Return Value

The root view of the content view hierarchy.

## Discussion

This content view defines the view hierarchy to be dimmed during incremental search, if the `NSTextFinder` instance’s incrementalSearchingShouldDimContentView is true. If this method is not implemented or returns `nil`, then the `NSTextFinder` instance will act as if incrementalSearchingShouldDimContentView is false

## See Also

### Find Bar View

var findBarView: NSView?

The view assigned by the text bar as the find bar view for the container.

**Required**

var isFindBarVisible: Bool

Returns whether the container should display its find bar.

**Required**

