

- UIKit
-  UIDocumentBrowserViewController 

Class

# UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDocumentBrowserViewController
```

## Mentioned in 

Providing access to directories

Customizing the browser

## Overview

With the document browser view controller, users can easily access and view their documents in the cloud. By default, the document browser can access both the system’s local file provider and its iCloud file provider.

The local file provider grants access to all the documents in the app’s `Documents` directory. Users can also access documents from another app’s `Documents` directory, if that app declares either the UISupportsDocumentBrowser key, or both the UIFileSharingEnabled and LSSupportsOpeningDocumentsInPlace keys in its `Info.plist` file. When the user opens a document from another app’s `Documents` directory, they edit the document in place, and save the changes to the other app’s `Documents` directory.

The iCloud file provider creates a folder for your app in the user’s iCloud Drive. Users can access documents from this folder, or from anywhere in their iCloud Drive. The system automatically handles access to iCloud for you, so you don’t need to enable your app’s iCloud capabilities.

Third-party storage services can also provide access to the documents they manage by implementing a File Provider extension (iOS 11 or later). For more information, see File Provider.

Important

Don’t assume that the files you access are local. Users can store files in iCloud Drive, or in any cloud storage that provides a current File Provider extension.

Remember that the system (or other apps) might modify the files that the document browser provides at any time. Therefore, you must coordinate your access to these files using either a UIDocument subclass, or NSFilePresenter and NSFileCoordinator objects.

## Topics

### Creating a document browser

Adding a document browser to your app

Give users access to their local or remote documents from within your app.

init(forOpening: [UTType]?)

Initializes and returns a document browser view controller that can open the specified file types.

### Creating new documents

var activeDocumentCreationIntent: UIDocument.CreationIntent?

The current intent that defines how your app creates a document.

### Responding to browser events

var delegate: (any UIDocumentBrowserViewControllerDelegate)?

The document browser’s delegate.

protocol UIDocumentBrowserViewControllerDelegate

The protocol you implement to respond as the user interacts with the document browser.

func importDocument(at: URL, nextToDocumentAt: URL, mode: UIDocumentBrowserViewController.ImportMode, completionHandler: (URL?, (any Error)?) -> Void)

Imports a document into the same location as an existing document.

### Configuring a document browser

var allowsDocumentCreation: Bool

A Boolean value that determines whether the document browser can create new documents.

var allowsPickingMultipleItems: Bool

A Boolean value that determines whether the user can select and open more than one document at a time.

func revealDocument(at: URL, importIfNeeded: Bool, completion: ((URL?, (any Error)?) -> Void)?)

Reveals, and optionally imports, the document at the provided URL.

var contentTypesForRecentDocuments: [UTType]

Content types for browsing recent documents.

### Modifying the browser’s appearance

var browserUserInterfaceStyle: UIDocumentBrowserViewController.BrowserUserInterfaceStyle

The visual style for the document browser.

enum BrowserUserInterfaceStyle

Styles that define the document browser’s appearance.

var additionalLeadingNavigationBarButtonItems: [UIBarButtonItem]

Additional bar button items that the document browser displays on the leading side of its navigation bar.

var additionalTrailingNavigationBarButtonItems: [UIBarButtonItem]

Additional bar button items that the document browser displays on the trailing side of its navigation bar.

var shouldShowFileExtensions: Bool

A Boolean value that determines whether the browser always shows file extensions.

var localizedCreateDocumentActionTitle: String

The title for the Create Document button.

var defaultDocumentAspectRatio: CGFloat

The aspect ratio for the Create Document button.

### Adding custom actions

var customActions: [UIDocumentBrowserAction]

Custom document browser actions.

class UIDocumentBrowserAction

A custom action that you can create and add to a document browser’s Edit menu or navigation bar.

### Animating transitions

func transitionController(forDocumentAt: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

class UIDocumentBrowserTransitionController

An object that implements the standard loading and transition animations for a document browser.

### Renaming a document

func renameDocument(at: URL, proposedName: String, completionHandler: (URL?, (any Error)?) -> Void)

Renames a document at the specified URL.

### Handling errors

struct UIDocumentBrowserError

A structure that contains information about document browser errors.

enum Code

The error codes for document browser errors.

let UIDocumentBrowserErrorDomain: String

The error domain for document browser errors.

### Deprecated symbols

init(forOpeningFilesWithContentTypes: [String]?)

Initializes and returns a document browser view controller that can open the specified file types.

Deprecated

var recentDocumentsContentTypes: [String]

Content types for browsing recent documents.

Deprecated

var allowedContentTypes: [String]

The document types that the browser can open.

Deprecated

func transitionController(forDocumentURL: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

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

class UIDocumentPickerViewController

A view controller that provides access to documents or destinations outside your app’s sandbox.

class UIDocumentInteractionController

A view controller that previews, opens, or prints files with a file format that your app can’t handle directly.

