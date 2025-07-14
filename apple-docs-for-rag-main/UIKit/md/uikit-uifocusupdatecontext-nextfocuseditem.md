

- UIKit
- UIFocusUpdateContext
-  nextFocusedItem 

Instance Property

# nextFocusedItem

The item to be focused after the update.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var nextFocusedItem: (any UIFocusItem)? { get }
```

## Discussion

This property is set to `nil` if no item is receiving the focus.

## See Also

### Getting related focus items

var previouslyFocusedItem: (any UIFocusItem)?

The item that was focused before the update.

