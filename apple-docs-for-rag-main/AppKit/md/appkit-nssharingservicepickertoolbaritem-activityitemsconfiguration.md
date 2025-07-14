

- AppKit
- NSSharingServicePickerToolbarItem
-  activityItemsConfiguration 

Instance Property

# activityItemsConfiguration

The custom object from an app built with Mac Catalyst that provides the items to share.

Mac Catalyst 13.0+

``` source
@MainActor
var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)? { get set }
```

## Discussion

Use this object to provide the set of items to share from your macOS window.

## See Also

### Getting the Toolbar Items

var delegate: (any NSSharingServicePickerToolbarItemDelegate)?

The custom object from your app that provides the items to share.

protocol NSSharingServicePickerToolbarItemDelegate

An interface that provides the content to share from the macOS share sheet.

