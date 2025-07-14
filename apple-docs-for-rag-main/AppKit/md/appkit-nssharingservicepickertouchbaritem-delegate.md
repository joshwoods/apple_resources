

- AppKit
- NSSharingServicePickerTouchBarItem
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the sharing service picker bar item.

macOS 10.12.2+

``` source
@MainActor
weak var delegate: (any NSSharingServicePickerTouchBarItemDelegate)? { get set }
```

## See Also

### Setting the delegate

protocol NSSharingServicePickerTouchBarItemDelegate

A protocol that a sharing service picker item delegate uses to provide a list of items eligible for sharing.

