

- AppKit
-  NSPreviewRepresentableActivityItem 

Protocol

# NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

macOS 13.0+

``` source
protocol NSPreviewRepresentableActivityItem : NSObjectProtocol
```

## Overview

Adopt the NSPreviewRepresentableActivityItem interface in custom types your app makes available for sharing. Use this protocol to specify the item itself and a title and image the share sheet can use to create a preview for your item. To share the item from your app, initialize the NSSharingServicePicker object with the object that adopts this protocol.

Note

If your data consists of standard types like strings or images, use an NSPreviewRepresentingActivityItem object to specify metadata for those types. If your data consists of URLs, pass them directly to the sharing service picker instead of creating a custom preview item.

## Topics

### Providing the Item to Share

var item: Any

The app-specific item you want to share.

**Required**

### Providing Metadata About the Item

var title: String?

A localized string that contains the name of the item.

var imageProvider: NSItemProvider?

An object that provides a visual representation of the item.

var iconProvider: NSItemProvider?

An object that provides an icon that represents the item’s source.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSPreviewRepresentingActivityItem

## See Also

### App Services

class NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

class NSSharingServicePicker

A list of sharing services that the user can choose from.

class NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

protocol NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

Services Functions

Configure the contents of your app’s Services menu.

