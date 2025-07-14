

- UIKit
-  App extensions 

API Collection

# App extensions

Extend your app’s basic functionality to other parts of the system.

## Topics

### Extension support

Use these Foundation classes to manage interactions between your app extension and its hosting app.

protocol NSExtensionRequestHandling : NSObjectProtocol

The interface an app extension uses to respond to a request from a host app.

class NSExtensionContext

The host app context from which an app extension is invoked.

### Document provider

class NSFileProviderExtension

The principal class for the nonreplicated File Provider extension.

class UIDocumentPickerExtensionViewController

The principal class for the Document Picker View Controller extension.

Deprecated

### Custom keyboard

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

protocol UIInputViewAudioFeedback

A property that enables a custom input or keyboard accessory view to play standard keyboard input clicks.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

## See Also

### App structure

App and environment

Manage life-cycle events and your app’s UI scenes, and get information about traits and the environment in which your app runs.

Documents, data, and pasteboard

Organize your app’s data and share that data on the pasteboard.

Resource management

Manage the images, strings, storyboards, and nib files that you use to implement your app’s interface.

Interprocess communication

Display activity-based services to people.

Mac Catalyst

Create a version of your iPad app that users can run on a Mac device.

