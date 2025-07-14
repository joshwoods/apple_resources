

- Safari Services
-  SFSafariApplication 

Class

# SFSafariApplication

A proxy for the Safari app.

macOS 10.12+

``` source
class SFSafariApplication
```

## Overview

The `SFSafariApplication` class is used by a Safari app extension to access the active Safari window, open a new window, and update the toolbar items on a window. An application that acts as a host container for a Safari app extension can use this class to send messages to the app extension. There is no object instance for this class.

## Topics

### Communicating With the App Extension

class func dispatchMessage(withName: String, toExtensionWithIdentifier: String, userInfo: [String : Any]?, completionHandler: (((any Error)?) -> Void)?)

Sends a message to a Safari app extension, launching Safari if necessary.

### Working with Windows

class func getActiveWindow(completionHandler: (SFSafariWindow?) -> Void)

Calls the completion handler with the active browser window.

class func openWindow(with: URL, completionHandler: ((SFSafariWindow?) -> Void)?)

Opens a new window with the desired webpage.

class func showPreferencesForExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Launches Safari and opens the preferences panel for a Safari app extension.

### Updating Toolbar Items

class func setToolbarItemsNeedUpdate()

Updates the enabled states and badges of toolbar items.

### Type Methods

class func getAllWindows(completionHandler: ([SFSafariWindow]) -> Void)

class func getHostApplication(completionHandler: (NSRunningApplication) -> Void)

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

## See Also

### Safari app extensions

Safari app extensions

Learn how Safari app extensions extend the web-browsing experience in Safari by leveraging web technologies and native code.

class SFSafariExtension

A proxy for the Safari extension.

class SFSafariWindow

A proxy for a Safari window.

class SFSafariPage

A proxy for a Safari webpage.

class SFSafariTab

A proxy for a tab in a Safari window.

