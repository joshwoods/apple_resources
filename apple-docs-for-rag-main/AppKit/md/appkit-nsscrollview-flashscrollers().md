

- AppKit
- NSScrollView
-  flashScrollers() 

Instance Method

# flashScrollers()

Flash the overlay scroll bars.

macOS 10.7+

``` source
@MainActor
func flashScrollers()
```

## Discussion

This method only applies to scroll views that use overlay scrollers.

This method can be invoked to cause the overlay scroller knobs to be momentarily shown. This may be desirable when changing a document view’s size or swapping new content into the view, or to give the user a sense of the current position within the scrollable range at each step of an incremental search or similar operation.

