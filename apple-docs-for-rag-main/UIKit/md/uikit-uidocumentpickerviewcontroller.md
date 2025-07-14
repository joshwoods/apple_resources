

- UIKit
-  UIDocumentPickerViewController 

Class

# UIDocumentPickerViewController

A view controller that provides access to documents or destinations outside your app’s sandbox.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDocumentPickerViewController
```

## Mentioned in 

Providing access to directories

## Overview

Use a document picker view controller to select a document to open or export, and optionally copy. Don’t copy the document if you can avoid it. The document picker operates in two modes:

- Open a document. The user selects a document. The document picker provides access to the document, and the user can edit the document in place. Optionally, you can specify that the document picker makes a copy of the document, leaving the original unchanged.

- Export a local document. The user selects a destination. The document picker moves the document, and the user can access it and edit it in place. Optionally, you can specify that the document picker makes a copy of the document, leaving the original unchanged.

### Work with external documents

Both the open and export operations grant access to documents outside your app’s sandbox. This access gives users an unprecedented amount of flexibility when working with their documents. However, it also adds a layer of complexity to your file handling. External documents have the following additional requirements:

- The open and move operations provide security-scoped URLs for all external documents. Call the startAccessingSecurityScopedResource() method to access or bookmark these documents, and the stopAccessingSecurityScopedResource() method to release them. If you’re using a `UIDocument` subclass to manage your document, it automatically manages the security-scoped URL for you.

- Always use file coordinators (see NSFileCoordinator) to read and write to external documents.

- Always use a file presenter (see NSFilePresenter) when displaying the contents of an external document.

- Don’t save URLs that the open and move operations provide. You can, however, save a bookmark to these URLs after calling startAccessingSecurityScopedResource() to ensure you have access. Call the bookmarkData(options:includingResourceValuesForKeys:relativeTo:) method and pass in the withSecurityScope option, creating a bookmark that contains a security-scoped URL.

For more information about working with external documents, see Providing access to directories and Adding a document browser to your app.

## Topics

### Creating a document picker

init?(coder: NSCoder)

Returns an initialized object from data in a specified unarchiver.

convenience init(forExporting: [URL])

Creates and returns a document picker that can export the types of documents you specify.

init(forExporting: [URL], asCopy: Bool)

Creates and returns a document picker that can export or copy the types of documents you specify.

convenience init(forOpeningContentTypes: [UTType])

Creates and returns a document picker that can open the types of documents you specify.

init(forOpeningContentTypes: [UTType], asCopy: Bool)

Creates and returns a document picker that can open or copy the types of documents you specify.

### Getting the user-selected document

var delegate: (any UIDocumentPickerDelegate)?

An object that acts as the delegate of the view controller.

protocol UIDocumentPickerDelegate

A set of methods for tracking when the user selects a document or destination, or cancels the operation.

var allowsMultipleSelection: Bool

A Boolean value that determines whether the user can select more than one document at a time.

var directoryURL: URL?

The initial directory that the document picker displays.

### Configuring a document picker

var shouldShowFileExtensions: Bool

A Boolean value that determines whether the browser always shows file extensions.

var documentPickerMode: UIDocumentPickerMode

The type of file transfer operation that the document picker uses.

Deprecated

enum UIDocumentPickerMode

Modes that define the type of file transfer operation that the document picker uses.

Deprecated

### Deprecated

init(documentTypes: [String], in: UIDocumentPickerMode)

Creates and returns a document picker that can open or copy the specified file types.

Deprecated

init(url: URL, in: UIDocumentPickerMode)

Initializes and returns a document picker that can export or copy the specified document.

Deprecated

init(urls: [URL], in: UIDocumentPickerMode)

Creates and returns a document picker that can export or move the specified documents.

Deprecated

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

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

class UIDocumentInteractionController

A view controller that previews, opens, or prints files with a file format that your app can’t handle directly.

