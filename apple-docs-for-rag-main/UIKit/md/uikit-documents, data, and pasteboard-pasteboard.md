

- UIKit
-  Documents, data, and pasteboard 

API Collection

# Documents, data, and pasteboard

Organize your app’s data and share that data on the pasteboard.

## Topics

### Documents

class UIDocument

An abstract base class for managing discrete portions of your app’s data.

class UIManagedDocument

A managed document object that integrates with Core Data.

Synchronizing documents in the iCloud environment

Manage documents across multiple devices to create a seamless editing and collaboration experience.

### Document presentation

class UIDocumentViewController

A view controller that manages and presents a document stored locally or in the cloud.

### Data management

protocol UIDataSourceModelAssociation

A set of methods that defines an interface for providing persistent references to data objects in your app.

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

## See Also

### App structure

App and environment

Manage life-cycle events and your app’s UI scenes, and get information about traits and the environment in which your app runs.

Resource management

Manage the images, strings, storyboards, and nib files that you use to implement your app’s interface.

App extensions

Extend your app’s basic functionality to other parts of the system.

Interprocess communication

Display activity-based services to people.

Mac Catalyst

Create a version of your iPad app that users can run on a Mac device.

