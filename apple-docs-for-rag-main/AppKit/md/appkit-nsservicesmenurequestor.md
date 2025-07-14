

- AppKit
-  NSServicesMenuRequestor 

Protocol

# NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

macOS

``` source
protocol NSServicesMenuRequestor : NSObjectProtocol
```

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Overview

This informal protocol consists of two methods, writeSelection(to:types:) and readSelection(from:). The first method provides data to a remote service, and the second receives any data the remote service might send back. Both respond to messages that are generated when the user chooses a command from the Services menu.

## Topics

### Working with Pasteboards

func readSelection(from: NSPasteboard) -> Bool

Reads data from the pasteboard and uses it to replace the current selection.

func writeSelection(to: NSPasteboard, types: [NSPasteboard.PasteboardType]) -> Bool

Writes the current selection to the pasteboard.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### App Services

class NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

class NSSharingServicePicker

A list of sharing services that the user can choose from.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

class NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

Services Functions

Configure the contents of your app’s Services menu.

