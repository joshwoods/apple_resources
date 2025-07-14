

- AppKit
- NSMenuDelegate
-  menuHasKeyEquivalent(\_:for:target:action:) 

Instance Method

# menuHasKeyEquivalent(\_:for:target:action:)

Invoked to allow the delegate to return the target and action for a key-down event.

macOS 10.0+

``` source
@MainActor
optional func menuHasKeyEquivalent(
    _ menu: NSMenu,
    for event: NSEvent,
    target: AutoreleasingUnsafeMutablePointer,
    action: UnsafeMutablePointer
) -> Bool
```

## Parameters 

`menu`  

The menu object sending the delegation message.

`event`  

An NSEvent object representing a key-down event.

`target`  

Return by reference the target object for the menu item that corresponds to the event. Specify `nil` to request the menu’s target.

`action`  

Return by reference the action selector for the menu item that corresponds to the event.

## Return Value

If there is a valid and enabled menu item that corresponds to this key-down even, return true after specifying the target and action. Return false if there are no items with that key equivalent or if the item is disabled.

## Discussion

If the delegate doesn’t define this method, the menu is populated to find out if any items have a matching key equivalent.

## See Also

### Related Documentation

func performActionForItem(at: Int)

Causes the application to send the action message of a specified menu item to its target.

Application Menu and Pop-up List Programming Topics

func performKeyEquivalent(with: NSEvent) -> Bool

Performs the action for the menu item that corresponds to the given key equivalent.

