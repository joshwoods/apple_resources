

- UIKit
- UIFocusUpdateContext
-  previouslyFocusedItem 

Instance Property

# previouslyFocusedItem

The item that was focused before the update.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var previouslyFocusedItem: (any UIFocusItem)? { get }
```

## Discussion

This property is set to `nil` when there was no previously focused item.

## See Also

### Getting related focus items

var nextFocusedItem: (any UIFocusItem)?

The item to be focused after the update.

