

- AppKit
-  NSHelpManager 

Class

# NSHelpManager

An object for displaying online help for an app.

macOS

``` source
@MainActor
class NSHelpManager
```

## Overview

The NSHelpManager class provides an approach to displaying online help. An app contains one NSHelpManager object.

## Topics

### Getting the Help Manager

class var shared: NSHelpManager

Returns the shared NSHelpManager instance, creating it if it does not already exist.

### Displaying Help

func find(String, inBook: NSHelpManager.BookName?)

Performs a search for the specified string in the specified book.

func openHelpAnchor(NSHelpManager.AnchorName, inBook: NSHelpManager.BookName?)

Finds and displays the text at the given anchor location in the given book.

typealias AnchorName

typealias BookName

### Dynamically Adding Help Books

func registerBooks(in: Bundle) -> Bool

Registers one or more help books in the given bundle.

### Configuring Context-Sensitive Help

func setContextHelp(NSAttributedString, for: Any)

Associates help content with an object.

func removeContextHelp(for: Any)

Removes the association between an object and its context-sensitive help.

### Displaying Context-Sensitive Help

func contextHelp(for: Any) -> NSAttributedString?

Returns context-sensitive help for an object.

func showContextHelp(for: Any, locationHint: NSPoint) -> Bool

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

typealias ContextHelpKey

class var isContextHelpModeActive: Bool

### Notifications

class let contextHelpModeDidActivateNotification: NSNotification.Name

Posted when the application enters context-sensitive help mode. This typically happens when the user holds down the Help key.

class let contextHelpModeDidDeactivateNotification: NSNotification.Name

Posted when the application exits context-sensitive help mode. This happens when the user clicks the mouse button while the cursor is anywhere on the screen after displaying a context-sensitive help topic.

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
- Sendable

## See Also

### App Help

protocol NSUserInterfaceItemSearching

A set of methods an app can implement to provide Spotlight for Help for its own custom help data.

