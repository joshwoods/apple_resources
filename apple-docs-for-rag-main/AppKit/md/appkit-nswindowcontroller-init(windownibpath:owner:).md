

- AppKit
- NSWindowController
-  init(windowNibPath:owner:) 

Initializer

# init(windowNibPath:owner:)

Returns a window controller initialized with a nib file at an absolute path and a specified owner.

macOS

``` source
@MainActor
convenience init(
    windowNibPath: String,
    owner: Any
)
```

## Parameters 

`windowNibPath`  

The full path to the nib file that archives the receiver’s window; cannot be `nil`.

`owner`  

The nib file’s owner; cannot be `nil`.

## Discussion

Use this method if your nib file is at a fixed location (which is not inside either the file’s owner’s class’s bundle or in the application’s main bundle). The default initialization turns on cascading, sets the shouldCloseDocument property to false, and sets the autosave name for the window’s frame to an empty string.

## See Also

### Initializing Window Controllers

init(window: NSWindow?)

Returns a window controller initialized with a given window.

convenience init(windowNibName: NSNib.Name)

Returns a window controller initialized with a nib file.

convenience init(windowNibName: NSNib.Name, owner: Any)

Returns a window controller initialized with a nib file and a specified owner for that nib file.

