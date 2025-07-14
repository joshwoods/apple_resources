

- AppKit
-  NSWindowRestoration 

Protocol

# NSWindowRestoration

A set of methods that restoration classes must implement to handle the recreation of windows.

macOS

``` source
protocol NSWindowRestoration : NSObjectProtocol
```

## Overview

At launch time, the application object retrieves the restoration class and uses its restoreWindow(withIdentifier:state:completionHandler:) method to obtain a new window whose type matches the type that was preserved previously. Classes that adopt this protocol can use the provided information to create (or obtain a reference to) the window in the new application. As part of creating the window, the class should also create any related objects, such as window controllers, normally used to manage the window.

## Topics

### Handling Window Restoration

static func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void)

Asks the class to provide a new window for the specified identifier.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSDocumentController

## See Also

### Window Restoration

protocol NSUserInterfaceItemIdentification

A set of methods used to associate a unique identifier with objects in your user interface.

