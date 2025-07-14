

- AppKit
- NSWindowController
-  init(window:) 

Initializer

# init(window:)

Returns a window controller initialized with a given window.

macOS

``` source
@MainActor
init(window: NSWindow?)
```

## Parameters 

`window`  

The window object to manage; can be `nil`.

## Return Value

A newly initialized window controller.

## Discussion

This method is the designated initializer for `NSWindowController`.

This initializer is useful when a window has been loaded but no window controller is assigned. The default initialization turns on cascading, sets the shouldCloseDocument property to false, and sets the window frame autosave name to an empty string. As a side effect, the created window controller is added as an observer of the willCloseNotifications posted by that window object (which is handled by a private method). If you make the window controller a delegate of the window, you can implement NSWindow’s windowShouldClose: delegate method.

## See Also

### Related Documentation

Document-Based App Programming Guide for Mac

### Initializing Window Controllers

convenience init(windowNibName: NSNib.Name)

Returns a window controller initialized with a nib file.

convenience init(windowNibName: NSNib.Name, owner: Any)

Returns a window controller initialized with a nib file and a specified owner for that nib file.

convenience init(windowNibPath: String, owner: Any)

Returns a window controller initialized with a nib file at an absolute path and a specified owner.

