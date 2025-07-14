

- UIKit
-  UIDocument 

Class

# UIDocument

An abstract base class for managing discrete portions of your app’s data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDocument
```

## Mentioned in 

Customizing a document-based app’s launch experience

About App Development with UIKit

## Overview

Apps that make use of UIDocument and its underlying architecture get many benefits for their documents:

- Asynchronous reading and writing of data on a background queue, meaning your app’s responsiveness is unaffected while reading and writing operations take place

- Coordinated reading and writing of document files automatically integrated with cloud services

- Support for discovering conflicts between different versions of a document

- Safe-saving of document data by writing data first to a temporary file and then replacing the current document file with it

- Automatic saving of document data at opportune moments and support for dealing with suspend behaviors

In the Model-View-Controller design pattern, a UIDocument object is a model object or model-controller object — it manages the data of a document or the aggregate model objects that together constitute the document’s data. You typically pair it with a view controller that manages the view presenting the document’s contents. UIDocument provides no direct support for managing document views, but view controllers that subclass UIDocumentViewController can present a `UIDocument`, and view controllers that subclass UIDocumentBrowserViewController can organize and display `UIDocument` collections.

Document-based apps include those that can generate multiple documents, each with its own file-system location. A document-based app must create a subclass of UIDocument for its documents.

Note

If you’re using a database to store document data, create a subclass of the UIManagedDocument class instead of UIDocument; UIManagedDocument is a subclass of UIDocument.

The primary attribute of a document in the UIDocument architecture is its file URL. When you initialize an instance of your document subclass by calling init(fileURL:), you must pass a file URL locating the document file in the app sandbox. UIDocument determines the file type (the Uniform Type Identifier associated with the file extension) and the document name (the filename component) from the file URL. You can override the accessor methods of the fileType and localizedName properties to supply different values.

The following outlines the life cycle of a typical document:

1.  You create a new document or open an existing document.

    - To create a new document, allocate and initialize an instance of your subclass and then call save(to:for:completionHandler:) on the instance.

    - To open an existing document (selected by the user), allocate and initialize an instance of your subclass and then call open(completionHandler:) on the instance.

2.  The user edits the document. As the user edits, track changes to the document. UIDocument periodically notes when there are unsaved changes and writes the document data to its file.

3.  The user requests that the document be integrated with cloud services (optional). You must enable the document for cloud storage. You must also resolve any conflicts between different versions of the same document.

4.  The user closes the document. Call close(completionHandler:) on the document instance. UIDocument saves the document if there are any unsaved changes.

A typical document-based app calls open(completionHandler:), close(completionHandler:), and save(to:for:completionHandler:) on the main thread. When the read or save operation kicked off by these methods concludes, the system executes the completion-handler block on the same dispatch queue as the system used to invoke the method, allowing you to complete any tasks contingent on the read or save operation. If the operation isn’t successful, the system passes false to the completion-handler block.

### Implement the NSFilePresenter protocol

The UIDocument class adopts the NSFilePresenter protocol. When another client attempts to read the document of a UIDocument-based app, the system suspends reading until the system provides the UIDocument object an opportunity to save any changes made to the document.

Although some implementations do nothing, UIDocument implements all NSFilePresenter methods. Specifically, UIDocument:

- Implements relinquishPresentedItem(toReader:) to forward the incoming block to performAsynchronousFileAccess(_:)

- Implements relinquishPresentedItem(toWriter:) to check if the file-modification date changed; if the file is newer than before, it calls revert(toContentsOf:completionHandler:) with the value of the fileURL as the URL parameter

- Implements presentedItemDidMove(to:) to update the document’s file URL (fileURL)

In your UIDocument subclass, if you override a NSFilePresenter method, you can always invoke the superclass implementation (`super`).

### Create a subclass

Each document-based app must create a subclass of UIDocument whose instances represent its documents. The subclassing requirements for most apps are simple:

- For writing operations, implement the contents(forType:) method to provide a snapshot of document data. The data must be in the form of an NSData object (for flat files) or an FileWrapper object (for file packages). Writing operations are usually initiated through the autosave feature.

- For reading operations, implement the load(fromContents:ofType:) method to receive an NSData or FileWrapper object and initialize the app’s data structures with it.

- Implement change tracking to enable the autosaving feature. See Track changes for details.

- When cloud services are enabled for a document, resolve conflicts between different versions of a document. See Resolve conflicts and handle errors for details.

  The system typically calls the contents(forType:) and load(fromContents:ofType:) methods on the main queue. More specifically:

- The system calls the contents(forType:) method on the queue that the system called the save(to:for:completionHandler:) method on; writing of data takes place on a background thread.

- The system calls the load(fromContents:ofType:) method on the queue that the system called the open(completionHandler:) method on.

If you have special requirements for reading and writing document data for which the contents(forType:) and load(fromContents:ofType:) methods won’t suffice, you can override other methods of the UIDocument class. See Override input and output methods for a discussion of these requirements and methods.

#### Track changes

To enable the autosaving feature of UIDocument, you must notify it when users make changes to a document. UIDocument periodically checks whether the hasUnsavedChanges method returns true; if it does, it initiates the save operation for the document.

There are two primary ways to implement change tracking in your UIDocument subclass:

- Call the methods of the UndoManager class to implement undo and redo for the document. You can access the default UndoManager object from the undoManager property. This is the preferred approach, especially for existing apps that already support undo and redo.

- Call the updateChangeCount(_:) method at the appropriate junctures in your code.

#### Resolve conflicts and handle errors

A UIDocument object has a specific state at any moment in its life cycle. You can check the current state by querying the documentState property, and get notified about changes by observing the stateChangedNotification notification.

If the owner enables a document for iCloud, it’s important to check for conflicting versions and to attempt to resolve conflicts. Listen for the stateChangedNotification notification and then checking if the document state is inConflict. This state indicates that there are conflicting versions of the document, which you can access by calling the NSFileVersion class method unresolvedConflictVersionsOfItem(at:), passing in the document’s file URL. If you can resolve a conflict correctly without user interaction, do so. Otherwise, discretely notify the user that a conflict exists and let them choose how to resolve it. Possible approaches include:

- Display the conflicting versions, from which a user can pick one or both versions to keep.

- Display a merged version and giving the user an option to pick it.

- Display the file modification dates and giving the user the option to choose one or both.

Document state, in addition to indicating an inter-file conflict, can indicate errors. For example, closed indicates an error in reading, and savingError indicates an error in saving or reverting a document. The system notifies your app of reading and writing errors through the `success` parameter passed into the completion handlers of the open(completionHandler:), close(completionHandler:), revert(toContentsOf:completionHandler:), and save(to:for:completionHandler:) methods.

You can handle errors by calling or implementing the handleError(_:userInteractionPermitted:) method; the default implementations of the open(completionHandler:) and save(to:for:completionHandler:) methods call `handleError(_:userInteractionPermitted:)` when a UIDocument object encounters a reading or writing error, respectively. You can handle read, save, and reversion errors by informing the user and, if the situation permits, trying to recover from the error.

Be sure to read the description for the contents(forType:) method for its guidance on handling errors encountered during document saving.

#### Override input and output methods

If you app has special requirements for reading or writing document data, it can override methods of UIDocument other than load(fromContents:ofType:) and contents(forType:). These requirements often include the following:

- Incremental reading and writing of large data files

  Override the read(from:) and writeContents(_:to:for:originalContentsURL:) methods, respectively.

- Custom representations of document data (that is, not an NSData or FileWrapper object)

  Override the read(from:) method when reading document data and the writeContents(_:to:for:originalContentsURL:) method when writing document data.

- Performing actions before or after reading or writing data

  Override open(completionHandler:) and save(to:for:completionHandler:).

- A custom approach to safe-saving

  Override the writeContents(_:andAttributes:safelyTo:for:) method.

- Changing the file type of a document before it’s saved

  Override the savingFileType method to return a file type other than the default (fileType). An example of this is an RTF document which, after a user adds an image to it, should be saved as an RTFD document.

If you override these methods, be aware that all reading and writing of document data must be done on a background queue and must be coordinated with other attempts to read from and write to the same document file. Because of this, you usually call the superclass implementation (`super`) as part of your override, and if you call other `UIDocument` methods, you usually invoke them in the block passed into a call of the performAsynchronousFileAccess(_:) method. Read the method descriptions for details.

#### Access document attributes

If you override any of the document-attribute properties (listed under Accessing document attributes) by overriding the related accessor methods, be aware that the UIKit framework can call these accessor methods on a background thread. Thus your overriding implementation must be thread safe.

### Rename documents

`UIDocument` provides support for changing the document’s title. Security considerations require that clients can’t programmatically rename a file on the file system, and that the system confirms that a person intends to rename their file. To satisfy these restrictions, the system, instead of your app, presents a renaming user interface using a process outside your app. The external process renames the underlying file and reports the new location back to the client.

To support this external process, `UIDocument` conforms to UINavigationItemRenameDelegate and handles the rename request internally when a person invokes renaming from the title menu. If you’re using UIDocumentViewController, it automatically configures renaming for you. Otherwise, you manually assign the document as the navigation item’s renameDelegate.

```
init(document: MyDocument) {
    self.document = document
    super.init(nibName:nil, bundle: nil)
    self.navigationItem.renameDelegate = document
}
```

The Rename action appears in the title menu as one of the system-suggested actions. When a person taps the Rename action, the system shows an inline text field for changing the navigation item’s `title`. Upon renaming the item, the system changes the file name in storage as though the person renamed the file in another application.

Prior to iOS 17, to enable the system rename user interface, a client view controller adopts the `UINavigationItemRenameDelegate` protocol and assigns itself as the navigation item’s `renameDelegate`. It’s the client’s responsibility to implement callbacks such as navigationItem(_:didEndRenamingWith:) (Swift) or navigationItem:didEndRenamingWithTitle: (Objective-C) to explicitly move the file in storage.

```
class EditorViewController: UIViewController,
        UINavigationItemRenameDelegate {

    override func viewDidLoad() {
        super.viewDidLoad()
        navigationItem.renameDelegate = self
    }

    func navigationItem(_ navigationItem: UINavigationItem, didEndRenamingWith: title: String) {
        // Move the file, update the model, and so on.
    }
}
```

## Topics

### Initializing a document object

init(fileURL: URL)

Returns a document object initialized with its file-system location.

### Accessing document attributes

var fileURL: URL

The file URL you use to initialize the document.

var localizedName: String

The localized name of the document.

var fileType: String?

The file type of the document.

var fileModificationDate: Date?

The date and time your app last modified the document file.

var documentState: UIDocument.State

The current state of the document.

var progress: Progress?

The upload or download progress of a document.

### Writing document data

func close(completionHandler: ((Bool) -> Void)?)

Asynchronously closes the document after saving any changes.

func contents(forType: String) throws -> Any

Returns the document data to be saved.

func save(to: URL, for: UIDocument.SaveOperation, completionHandler: ((Bool) -> Void)?)

Saves document data to the specified location in the application sandbox.

func writeContents(Any, andAttributes: [AnyHashable : Any]?, safelyTo: URL, for: UIDocument.SaveOperation) throws

Ensures that document data is written safely to a specified location in the application sandbox.

func writeContents(Any, to: URL, for: UIDocument.SaveOperation, originalContentsURL: URL?) throws

Writes the document data to disk at the sandbox location indicated by a file URL.

var savingFileType: String?

Returns the file type to use for saving a document.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.

### Reading document data

func open(completionHandler: ((Bool) -> Void)?)

Opens a document asynchronously.

func load(fromContents: Any, ofType: String?) throws

Loads the document data into the app’s data model.

func read(from: URL) throws

Reads the document data in a file at a specified location in the application sandbox.

### Creating new documents

struct CreationIntent

An app intent that creates new documents for your app.

### Accessing document files asynchronously

func performAsynchronousFileAccess(() -> Void)

Schedules a document-reading or document-writing operation on a concurrent background queue.

### Reverting a document

func revert(toContentsOf: URL, completionHandler: ((Bool) -> Void)?)

Reverts a document to the most recent document data stored on-disk.

### Disabling and enabling editing

func disableEditing()

Disables editing when it’s unsafe to make changes to a document.

func enableEditing()

Enables editing when it’s safe again to make changes to a document.

### Tracking changes and autosaving

var hasUnsavedChanges: Bool

A Boolean value that indicates whether the document has any unsaved changes.

func updateChangeCount(UIDocument.ChangeKind)

Updates the change counter by indicating the kind of change.

var undoManager: UndoManager!

The undo manager for the document.

func changeCountToken(for: UIDocument.SaveOperation) -> Any

Returns a change token for a specific save operation.

func updateChangeCount(withToken: Any, for: UIDocument.SaveOperation)

Updates the change count with reference to a change-count token passed in by UIKit.

func autosave(completionHandler: ((Bool) -> Void)?)

Initiates automatic saving of documents with unsaved changes.

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this document.

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

### Resolving conflicts and handling errors

func handleError(any Error, userInteractionPermitted: Bool)

Handles an error that occurs during an attempt to read, save, or revert a document.

func finishedHandlingError(any Error, recovered: Bool)

Tells UIKit that you finished handling the error.

func userInteractionNoLongerPermitted(forError: any Error)

Indicates when it’s no longer safe to proceed without immediately handling the error.

### Constants

enum ChangeKind

Constants that specify the kind of change to a document.

enum SaveOperation

Constants that specify the type of save operation.

struct State

Constants that specify the document state.

class let userActivityURLKey: String

The key that identifies the document associated with a user activity.

### Notifications

class let stateChangedNotification: NSNotification.Name

A notification the document object posts when there’s a change in the state of the document.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIManagedDocument

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFilePresenter
- NSObjectProtocol
- ProgressReporting
- Sendable
- UIUserActivityRestoring

## See Also

### Documents

class UIManagedDocument

A managed document object that integrates with Core Data.

Synchronizing documents in the iCloud environment

Manage documents across multiple devices to create a seamless editing and collaboration experience.

