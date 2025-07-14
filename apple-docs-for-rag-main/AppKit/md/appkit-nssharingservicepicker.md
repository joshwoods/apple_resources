

- AppKit
-  NSSharingServicePicker 

Class

# NSSharingServicePicker

A list of sharing services that the user can choose from.

macOS 10.8+

``` source
class NSSharingServicePicker
```

## Overview

An NSSharingServicePicker object presents an interface for sharing one or more items using a specific service. In macOS 12 and earlier, this picker displays a menu with a list of services that someone can use to share the item. In macOS 13 and later, the picker displays a popover with a preview of the item and the list of services. When someone chooses a service, the picker automatically shares the proposed item with that service.

Create a sharing service picker and configure it with a delegate object to monitor interactions. Your delegate must conform to the NSSharingServicePickerDelegate protocol. Present the picker from your interface using the show(relativeTo:of:preferredEdge:) method.

## Topics

### Creating a sharing service picker

init(items: [Any])

Creates a new sharing service picker for the selected items.

### Managing the sharing service picker

var delegate: (any NSSharingServicePickerDelegate)?

The object for managing the sharing service picker.

protocol NSSharingServicePickerDelegate

An interface for managing content for the macOS share sheet.

### Displaying the sharing service picker

func show(relativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the picker interface and populates it with the relevant sharing services.

func close()

Closes the picker interface.

### Retrieving the sharing menu item

var standardShareMenuItem: NSMenuItem

A menu item suitable to display the picker for the specified items.

### Classes

class CollaborationModeRestriction

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### App Services

class NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

class NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

protocol NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

Services Functions

Configure the contents of your app’s Services menu.

