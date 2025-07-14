

- AppKit
-  NSSharingServicePickerTouchBarItemDelegate 

Protocol

# NSSharingServicePickerTouchBarItemDelegate

A protocol that a sharing service picker item delegate uses to provide a list of items eligible for sharing.

macOS

``` source
protocol NSSharingServicePickerTouchBarItemDelegate : NSSharingServicePickerDelegate
```

## Topics

### Providing items to share

func items(for: NSSharingServicePickerTouchBarItem) -> [Any]

Asks the delegate for items that represent the objects to be shared.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- NSSharingServicePickerDelegate

## See Also

### Setting the delegate

var delegate: (any NSSharingServicePickerTouchBarItemDelegate)?

The object that acts as the delegate of the sharing service picker bar item.

