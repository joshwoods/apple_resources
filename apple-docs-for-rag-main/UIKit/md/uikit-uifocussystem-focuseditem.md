

- UIKit
- UIFocusSystem
-  focusedItem 

Instance Property

# focusedItem

The item that’s currently focused.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
weak var focusedItem: (any UIFocusItem)? { get }
```

## Discussion

If the current object or none of its children are focused, this property is set to `nil`.

