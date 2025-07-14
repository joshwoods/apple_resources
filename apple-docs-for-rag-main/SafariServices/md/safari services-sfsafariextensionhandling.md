

- Safari Services
-  SFSafariExtensionHandling 

Protocol

# SFSafariExtensionHandling

A protocol for implementing event handling in a Safari app extension.

macOS 10.12+

``` source
protocol SFSafariExtensionHandling : NSObjectProtocol
```

## Topics

### Receiving Messages in Your App Extension

func messageReceived(withName: String, from: SFSafariPage, userInfo: [String : Any]?)

A method the system calls when the extension receives a message from an injected script.

func messageReceivedFromContainingApp(withName: String, userInfo: [String : Any]?)

A method the system calls when the extension receives a message from the extension’s containing app.

### Responding to Context Menu Selections

func contextMenuItemSelected(withCommand: String, in: SFSafariPage, userInfo: [String : Any]?)

A method the system calls when a user selects one of the app extension’s context menu items.

func validateContextMenuItem(withCommand: String, in: SFSafariPage, userInfo: [String : Any]?, validationHandler: (Bool, String?) -> Void)

Validates whether a particular contextual menu item should be displayed.

### Working with Toolbar Items

func toolbarItemClicked(in: SFSafariWindow)

A method the system calls when a user clicks a toolbar item associated with the app extension.

func validateToolbarItem(in: SFSafariWindow, validationHandler: (Bool, String) -> Void)

Determines if a toolbar menu item should be enabled or have badge text when browser state changes.

### Working with Popovers

func popoverViewController() -> SFSafariExtensionViewController

Asks the handler to provide a popover view controller for display.

func popoverWillShow(in: SFSafariWindow)

Tells the handler that the app extension’s popover is about to be opened.

func popoverDidClose(in: SFSafariWindow)

Tells the handler that the app extension’s popover was closed.

### Working with Content Blockers

func contentBlocker(withIdentifier: String, blockedResourcesWith: [URL], on: SFSafariPage)

Tells the handler which resources a content blocker blocked on a webpage.

### Responding to Page Navigation

func page(SFSafariPage, willNavigateTo: URL?)

A method the system calls when a webpage is about to navigate to a new URL.

### Instance Methods

func additionalRequestHeaders(for: URL, completionHandler: ([String : String]?) -> Void)

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SFSafariExtensionHandler

## See Also

### Related Documentation

class func dispatchMessage(withName: String, toExtensionWithIdentifier: String, userInfo: [String : Any]?, completionHandler: (((any Error)?) -> Void)?)

Sends a message to a Safari app extension, launching Safari if necessary.

### Injected style sheets and scripts

Using injected style sheets and scripts

Learn how you can affect the appearance or behavior of a webpage by using injected style sheets and scripts.

Injecting a script into a webpage

Inject a script that you write for a Safari app extension into a webpage.

Injecting CSS style sheets into a webpage

Add to or override styles by injecting CSS style sheets into webpages.

Passing messages between Safari app extensions and injected scripts

Communicate between your Safari app extension and injected scripts.

class SFSafariExtensionHandler

A base class that you subclass to handle events in your Safari app extension.

class SFSafariExtensionManager

A class that your app uses to find out the current state of a Safari app extension.

class SFSafariExtensionState

The state of a Safari app extension.

class SFSafariPageProperties

An object that captures information about a webpage.

let SFExtensionProfileKey: String

A string the system uses as a key in a user info dictionary to identify a profile identifier.

