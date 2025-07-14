

- AppKit
- NSTextFinder
-  cancelFindIndicator() 

Instance Method

# cancelFindIndicator()

Cancels the find indicator immediately.

macOS 10.7+

``` source
func cancelFindIndicator()
```

## Discussion

There may be some circumstances where the find indicator should be immediately cancelled or hidden, such as when the view’s content or selection is changed without the knowledge of the text finder. This method will immediately cancel the current find indicator.

The `NSTextFinder` and `NSView` classes will handle the find indicator correctly when a content view is resized, moved, or removed from the view hierarchy. If your content view’s scrolling is done by an `NSScrollView`, the find indicator will also be handled for you during scrolling.

## See Also

### Related Documentation

var findIndicatorNeedsUpdate: Bool

Invoke to specify that the find indicator needs updating when not contained within a scroll view.

### Validating and Performing Text Finding

func performAction(NSTextFinder.Action)

Performs the specified text finding action.

func validateAction(NSTextFinder.Action) -> Bool

Allows validation of the find action before performing.

