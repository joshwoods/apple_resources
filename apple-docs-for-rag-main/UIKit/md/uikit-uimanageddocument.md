

- UIKit
-  UIManagedDocument 

Class

# UIManagedDocument

A managed document object that integrates with Core Data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIManagedDocument
```

## Overview

UIManagedDocument is a concrete subclass of UIDocument. When you initialize a managed document, you specify the URL for the document location. The document object then creates a Core Data stack to use to access the document’s persistent store using a managed object model from the app’s main bundle. UIManagedDocument performs all the basic setup you need for Core Data, and in some cases you may use instances of the class directly (without a need to subclass). You can supply configuration options for the creation of the coordinator using persistentStoreOptions, and for the model using modelConfiguration. You can also perform additional customization by creating a subclass of UIManagedDocument:

- Override persistentStoreName to customize the name of the persistent store file inside the document’s file package.

- Override managedObjectModel to customize creation of the managed object model.

You do this if, for example, your app supports multiple document types, each of which uses a different model. You want to ensure that the models aren’t merged for each document class.

- Override persistentStoreType(forFileType:) to customize the type of persistent store used by a document.

- Override configurePersistentStoreCoordinator(for:ofType:modelConfiguration:storeOptions:) to customize the loading or creation of a persistent store.

### Handling errors

To enable your app to observe and handle errors in saving and validating a managed document, you must subclass the UIManagedDocument class and override one or both of the following two inherited methods from the UIDocument class:

- handleError(_:userInteractionPermitted:)

- finishedHandlingError(_:recovered:)

Overriding is required because otherwise, the only information your app receives on error is the stateChangedNotification notification, which doesn’t contain a `userInfo` dictionary and so doesn’t convey specific error information.

## Topics

### Managing the Core Data stack

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [AnyHashable : Any]?) throws

Creates or loads the document’s persistent store.

var managedObjectContext: NSManagedObjectContext

The document’s managed object context.

var managedObjectModel: NSManagedObjectModel

The document’s managed object model.

var persistentStoreOptions: [AnyHashable : Any]?

Options used when creating the document’s persistent store.

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

### Customizing read and write operations

func readAdditionalContent(from: URL) throws

Handles reading non-Core Data content in the additional content directory in the document’s file package.

func additionalContent(for: URL) throws -> Any

Handles writing non-Core Data content to the additional content directory in the document’s file package.

func writeAdditionalContent(Any, to: URL, originalContentsURL: URL?) throws

Handles writing non-Core Data content to the document’s file package.

### Naming the persistent store file

class var persistentStoreName: String

Returns the name for the persistent store file inside the document’s file package.

## Relationships

### Inherits From

- UIDocument

### Conforms To

- CVarArg
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

class UIDocument

An abstract base class for managing discrete portions of your app’s data.

Synchronizing documents in the iCloud environment

Manage documents across multiple devices to create a seamless editing and collaboration experience.

