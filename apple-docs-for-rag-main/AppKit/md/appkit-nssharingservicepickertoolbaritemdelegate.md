

- AppKit
-  NSSharingServicePickerToolbarItemDelegate 

Protocol

# NSSharingServicePickerToolbarItemDelegate

An interface that provides the content to share from the macOS share sheet.

macOS

``` source
protocol NSSharingServicePickerToolbarItemDelegate : NSSharingServicePickerDelegate
```

## Overview

Adopt the NSSharingServicePickerToolbarItemDelegate protocol in one of your app’s custom types and use it to provide shareable content. Assign your delegate object to an NSSharingServicePickerToolbarItem object you add to your window’s toolbar.

## Topics

### Providing the Items to Share

func items(for: NSSharingServicePickerToolbarItem) -> [Any]

Asks the delegate for the items to share.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- NSSharingServicePickerDelegate

## See Also

### Getting the Toolbar Items

var delegate: (any NSSharingServicePickerToolbarItemDelegate)?

The custom object from your app that provides the items to share.

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

The custom object from an app built with Mac Catalyst that provides the items to share.

