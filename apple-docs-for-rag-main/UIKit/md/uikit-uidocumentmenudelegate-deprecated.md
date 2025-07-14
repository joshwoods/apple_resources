

- UIKit
-  UIDocumentMenuDelegate Deprecated

Protocol

# UIDocumentMenuDelegate

A set of methods that you must implement to track user interactions with a document menu view controller.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
protocol UIDocumentMenuDelegate : NSObjectProtocol
```

## Overview

The document menu calls the methods of this protocol when the user selects a document picker or dismisses the menu. If the user selects a document picker, set the picker’s delegate and present it.

## Topics

### Responding to user actions

func documentMenu(UIDocumentMenuViewController, didPickDocumentPicker: UIDocumentPickerViewController)

Tells the delegate that the user has selected a document picker from the menu.

**Required**

func documentMenuWasCancelled(UIDocumentMenuViewController)

Tells the delegate that the user dismissed the document menu.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the user-selected document picker

var delegate: (any UIDocumentMenuDelegate)?

The document menu’s delegate.

Deprecated

