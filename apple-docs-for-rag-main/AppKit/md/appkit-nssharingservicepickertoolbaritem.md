

- AppKit
-  NSSharingServicePickerToolbarItem 

Class

# NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

iOS 10.13+iPadOS 10.13+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
class NSSharingServicePickerToolbarItem
```

## Overview

An NSSharingServicePickerToolbarItem object is a standard item you add to your window’s toolbar. When someone clicks it, the item displays the macOS share sheet. Use this item to share the selected or focal content from the current window. For example, you might share the photo someone is viewing, the currently selected text, or the window’s associated document.

Provide the items to share using the associated delegate object. For an app built using Mac Catalyst, provide the items from the object in the activityItemsConfiguration property.

## Topics

### Getting the Toolbar Items

var delegate: (any NSSharingServicePickerToolbarItemDelegate)?

The custom object from your app that provides the items to share.

protocol NSSharingServicePickerToolbarItemDelegate

An interface that provides the content to share from the macOS share sheet.

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

The custom object from an app built with Mac Catalyst that provides the items to share.

## Relationships

### Inherits From

- NSToolbarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSValidatedUserInterfaceItem
- Sendable

## See Also

### App Services

class NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

class NSSharingServicePicker

A list of sharing services that the user can choose from.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

protocol NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

Services Functions

Configure the contents of your app’s Services menu.

