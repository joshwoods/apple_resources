

- AppKit
-  NSSharingServicePickerDelegate 

Protocol

# NSSharingServicePickerDelegate

An interface for managing content for the macOS share sheet.

macOS

``` source
protocol NSSharingServicePickerDelegate : NSObjectProtocol
```

## Overview

Adopt the NSSharingServicePickerDelegate protocol in one of your app’s types, and use it to manage interactions with an NSSharingServicePicker object. Use your delegate object to customize the services for the proposed items and respond to the selection of a shared service.

For information about how to display the share sheet and configure your delegate, see NSSharingServicePicker.

## Topics

### Configuring the Sharing Services

func sharingServicePicker(NSSharingServicePicker, sharingServicesForItems: [Any], proposedSharingServices: [NSSharingService]) -> [NSSharingService]

Asks the delegate to specify which services to make available from the sharing service picker.

### Customizing Behavior

func sharingServicePicker(NSSharingServicePicker, didChoose: NSSharingService?)

Tells the delegate that the person selected a sharing service for the current item.

func sharingServicePicker(NSSharingServicePicker, delegateFor: NSSharingService) -> (any NSSharingServiceDelegate)?

Asks your delegate to provide an object that the selected sharing service can use as its delegate.

### Instance Methods

func sharingServicePickerCollaborationModeRestrictions(NSSharingServicePicker) -> [NSSharingServicePicker.CollaborationModeRestriction]?

Used to specify the case where the share picker should not support some modes of sharing even if they are supported by the items being shared. Disabling all possible modes at the same time is not supported behavior.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSSharingServicePickerToolbarItemDelegate
- NSSharingServicePickerTouchBarItemDelegate

## See Also

### Managing the sharing service picker

var delegate: (any NSSharingServicePickerDelegate)?

The object for managing the sharing service picker.

