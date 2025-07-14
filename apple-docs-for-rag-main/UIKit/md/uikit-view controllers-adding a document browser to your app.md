

- UIKit
- View controllers
-  Adding a document browser to your app 

# Adding a document browser to your app

Give users access to their local or remote documents from within your app.

## Overview

Use a document browser view controller as the root of your app’s view hierarchy. When a user selects a document, you present its view controller modally from your document browser.

Important

Always assign the document browser as your app’s root view controller. Don’t place the document browser in a navigation controller, tab bar, or split view, and don’t present the document browser modally.

If you want to present a document browser from another location in your view hierarchy, use a UIDocumentPickerViewController instead.

The browser automatically gives users the option to share documents using the Share button or a drag-and-drop action. It also provides a standard interface for browsing and managing documents.

You set the type of documents that the user can select when the browser is first created. You can also set the browser’s appearance, modify its behaviors, and add custom actions.

## Topics

### Configuration

Setting up a document browser app

Add a document browser view controller to your app.

Presenting selected documents

Display user-selected documents over your browser view controller.

Enabling document sharing

Give users the ability to import and export documents from your app.

### Customization

Customizing the browser

Customize the document browser’s look and behavior.

Adding custom actions and activities

Add custom document browser actions, activities, and bar items.

## See Also

### Documents and directories

Customizing a document-based app’s launch experience

Add unique elements to your app’s document launch scene.

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

class UIDocumentInteractionController

A view controller that previews, opens, or prints files with a file format that your app can’t handle directly.

