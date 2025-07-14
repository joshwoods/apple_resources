

- AppKit
-  Documents, Data, and Pasteboard 

API Collection

# Documents, Data, and Pasteboard

Organize your app’s data and preferences, and share that data on the pasteboard or in iCloud.

## Topics

### Documents

Developing a Document-Based App

Write an app that creates, manages, edits, and saves text documents.

class NSDocument

An abstract class that defines the interface for macOS documents.

class NSDocumentController

An object that manages an app’s documents.

class NSPersistentDocument

A document object that can integrate with Core Data.

### User Preferences

class NSUserDefaultsController

A controller that accesses user preference information for your app from the user’s defaults database.

class NSUbiquitousKeyValueStore

An iCloud-based container of key-value pairs you use to share data among instances of your app running on a user's connected devices.

### Pasteboard

class NSPasteboard

An object that transfers data to and from the pasteboard server.

class NSPasteboardItem

An item on a pasteboard.

protocol NSPasteboardReading

A set of methods that defines the interface for initializing an object from a pasteboard.

protocol NSPasteboardWriting

A set of methods that defines the interface for retrieving a representation of an object that can be written to a pasteboard.

protocol NSPasteboardItemDataProvider

A set of methods implemented by the data provider of a pasteboard item to provide the data for a particular UTI type.

struct ContentsOptions

Options for preparing the pasteboard.

protocol NSPasteboardTypeOwner

An object that serves as a data provider for data types that use lazy data fulfillment from a pasteboard request.

### File Promises

File promises support UTI-based drag and drop functions, including drag flocking. When possible, they’re pasteboard compliant and file coordinated.

Supporting Drag and Drop Through File Promises

Receive and provide file promises to support dragged app files and pasteboard operations.

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

class NSFilePromiseProvider

An object that provides a promise for the pasteboard.

protocol NSFilePromiseProviderDelegate

A set of methods that provides the name of the promised file and writes the file to the destination directory when the file promise is fulfilled.

class NSFilePromiseReceiver

An object that receives a file promise from the pasteboard.

### Object Editing

protocol NSEditor

protocol NSEditorRegistration

A set of methods that controllers can implement to enable an editor view to inform the controller when it has uncommitted changes.

## See Also

### App Structure

App and Environment

Learn about the objects that you use to interact with the system.

Cocoa Bindings

Automatically synchronize your data model with your app’s interface using Cocoa Bindings.

Resource Management

Manage the storyboards and nib files containing your app’s user interface, and learn how to load data that is stored in resource files.

App Extensions

Extend your app’s basic functionality to other parts of the system.

