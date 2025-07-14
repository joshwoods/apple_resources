

- AppKit
- NSMenu
-  delegate 

Instance Property

# delegate

The delegate of the menu.

macOS

``` source
weak var delegate: (any NSMenuDelegate)? { get set }
```

## Discussion

This property indicates the delegate of the menu.

You can use the delegate to populate a menu just before it is drawn and to check for key equivalents without creating a menu item.

## See Also

### Related Documentation

protocol NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

