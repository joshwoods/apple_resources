

- UIKit
- UIFocusItem
-  didHintFocusMovement(\_:) 

Instance Method

# didHintFocusMovement(\_:)

Indicates to the currently focused item that focus movement might occur.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
optional func didHintFocusMovement(_ hint: UIFocusMovementHint)
```

## Parameters 

`hint`  

The movement hint object corresponding to the user’s input.

## Discussion

The focus item is mutated by the focus engine whenever the user’s finger moves on the remote.

## See Also

### Providing movement hints

class UIFocusMovementHint

Provides movement hint information for the focused item.

