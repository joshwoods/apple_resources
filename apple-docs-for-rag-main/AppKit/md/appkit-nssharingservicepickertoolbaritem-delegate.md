

- AppKit
- NSSharingServicePickerToolbarItem
-  delegate 

Instance Property

# delegate

The custom object from your app that provides the items to share.

macOS 10.15+

``` source
@MainActor
weak var delegate: (any NSSharingServicePickerToolbarItemDelegate)? { get set }
```

## Discussion

Use your delegate object to provide the set of items you want to share from your window. If this property is `nil`, AppKit disables the toolbar item.

## See Also

### Getting the Toolbar Items

protocol NSSharingServicePickerToolbarItemDelegate

An interface that provides the content to share from the macOS share sheet.

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

The custom object from an app built with Mac Catalyst that provides the items to share.

