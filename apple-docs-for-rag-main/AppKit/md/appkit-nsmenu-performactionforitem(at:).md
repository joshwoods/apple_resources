

- AppKit
- NSMenu
-  performActionForItem(at:) 

Instance Method

# performActionForItem(at:)

Causes the application to send the action message of a specified menu item to its target.

macOS

``` source
func performActionForItem(at index: Int)
```

## Parameters 

`index`  

The integer index of a menu item.

## Discussion

If a target is not specified, the message is sent to the first responder. As a side effect, this method posts willSendActionNotification and didSendActionNotification.

In macOS 10.6 and later the `performActionForItemAtIndex:` no longer triggers menu validation. This is because validation is typically done during menu tracking or key equivalent matching, so the subsequent `performActionForItemAtIndex:` validation was redundant. To trigger validation explicitly, use invoke the update() method.

In OS X v10.6 `performActionForItemAtIndex:`, when called, now triggers highlighting in the menu bar. It also sends out appropriate accessibility notifications indicating the item was selected.

## See Also

### Related Documentation

func performKeyEquivalent(with: NSEvent) -> Bool

Performs the action for the menu item that corresponds to the given key equivalent.

