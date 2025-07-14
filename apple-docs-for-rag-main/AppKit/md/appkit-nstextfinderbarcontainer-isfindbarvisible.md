

- AppKit
- NSTextFinderBarContainer
-  isFindBarVisible 

Instance Property

# isFindBarVisible

Returns whether the container should display its find bar.

macOS

``` source
var isFindBarVisible: Bool { get set }
```

**Required**

## Discussion

When this property is true and the findBarView property is set, then the find bar is displayed by the container. Otherwise, the find bar is not displayed.

The default value should be false.

## See Also

### Find Bar View

var findBarView: NSView?

The view assigned by the text bar as the find bar view for the container.

**Required**

func contentView() -> NSView?

A view hierarchy that contains all the views which display the contents being searched.

