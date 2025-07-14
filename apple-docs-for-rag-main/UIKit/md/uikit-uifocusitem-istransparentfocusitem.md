

- UIKit
- UIFocusItem
-  isTransparentFocusItem 

Instance Property

# isTransparentFocusItem

Indicates if the focus item is transparent, which allows items behind it to become focused.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 18.0+visionOS 1.0+

``` source
@MainActor
optional var isTransparentFocusItem: Bool { get }
```

## Discussion

The system ignores this value when the item is focusable, in which case the item is never considered transparent.

