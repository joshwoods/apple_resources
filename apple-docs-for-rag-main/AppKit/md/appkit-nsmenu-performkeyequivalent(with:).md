

- AppKit
- NSMenu
-  performKeyEquivalent(with:) 

Instance Method

# performKeyEquivalent(with:)

Performs the action for the menu item that corresponds to the given key equivalent.

macOS

``` source
func performKeyEquivalent(with event: NSEvent) -> Bool
```

## Parameters 

`event`  

An NSEvent object that represents a key-equivalent event.

## Return Value

Returns true if `event` is a key equivalent that the menu should handle, otherwise returns false.

## See Also

### Related Documentation

func menuHasKeyEquivalent(NSMenu, for: NSEvent, target: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, action: UnsafeMutablePointer&lt;Selector?>) -> Bool

Invoked to allow the delegate to return the target and action for a key-down event.

func performActionForItem(at: Int)

Causes the application to send the action message of a specified menu item to its target.

