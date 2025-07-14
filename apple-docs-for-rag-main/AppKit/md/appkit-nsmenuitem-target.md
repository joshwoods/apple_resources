

- AppKit
- NSMenuItem
-  target 

Instance Property

# target

The menu item’s target.

macOS

``` source
weak var target: AnyObject? { get set }
```

## Discussion

To ensure that a menu item’s target can receive commands while a modal dialog is open, the target object should return true in worksWhenModal.

## See Also

### Managing the target and action

var action: Selector?

The menu item’s action-method selector.

