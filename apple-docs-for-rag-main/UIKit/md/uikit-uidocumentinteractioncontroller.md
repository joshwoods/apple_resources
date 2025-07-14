

- UIKit
-  UIDocumentInteractionController 

Class

# UIDocumentInteractionController

A view controller that previews, opens, or prints files with a file format that your app can’t handle directly.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDocumentInteractionController
```

## Overview

Use this class to present an appropriate user interface for previewing, opening, copying, or printing a specified file. For example, an email program might use this class to allow the user to preview attachments and open them in other apps.

After presenting its user interface, a document interaction controller handles all interactions needed to support file preview and menu display.

You can also use the delegate to participate in interactions occurring within the presented interface. For example, the delegate is notified when a file is about to be handed off to another application for opening. For a complete description of the methods you can implement in your delegate, see UIDocumentInteractionControllerDelegate.

## Topics

### Creating the document interaction controller

init(url: URL)

Creates a document interaction controller with the specified URL.

### Handling document-related interactions

var delegate: (any UIDocumentInteractionControllerDelegate)?

The delegate you want to receive document interaction notifications.

protocol UIDocumentInteractionControllerDelegate

A set of methods you can implement to respond to messages from a document interaction controller.

### Presenting and dismissing a document preview

func presentPreview(animated: Bool) -> Bool

Displays a full-screen preview of the target document.

func dismissPreview(animated: Bool)

Dismisses the currently active document preview.

### Presenting and dismissing menus

func presentOptionsMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified location in the view.

func presentOptionsMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified bar button item.

func presentOpenInMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified view.

func presentOpenInMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified bar button item.

func dismissMenu(animated: Bool)

Dismisses the currently active menu.

### Accessing the target document’s attributes

var url: URL?

The URL identifying the target file on the local filesystem.

var uti: String?

The type of the target file.

var name: String?

The name of the target file.

var icons: [UIImage]

The images associated with the target file.

var annotation: Any?

Custom property list information for the target file.

### Accessing the controller attributes

var gestureRecognizers: [UIGestureRecognizer]

The system-supplied gesture recognizers for presenting a document interaction controller.

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
- Sendable
- UIActionSheetDelegate

## See Also

### Documents and directories

Customizing a document-based app’s launch experience

Add unique elements to your app’s document launch scene.

Adding a document browser to your app

Give users access to their local or remote documents from within your app.

Providing access to directories

Use a document picker to access the content of a directory outside your app’s container.

Building a document browser-based app

Use a document browser to provide access to the user’s text files.

Building a document browser app for custom file formats

Implement a custom document file format to manage user interactions with files on different cloud storage providers.

class UIDocumentViewController

A view controller that manages and presents a document stored locally or in the cloud.

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

class UIDocumentPickerViewController

A view controller that provides access to documents or destinations outside your app’s sandbox.

