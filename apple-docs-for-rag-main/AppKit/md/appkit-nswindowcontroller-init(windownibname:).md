

- AppKit
- NSWindowController
-  init(windowNibName:) 

Initializer

# init(windowNibName:)

Returns a window controller initialized with a nib file.

macOS

``` source
@MainActor
convenience init(windowNibName: NSNib.Name)
```

## Parameters 

`windowNibName`  

The name of the nib file (minus the “`.nib`” extension) that archives the receiver’s window; cannot be `nil`.

## Discussion

Sets the owner of the nib file to the receiver. The default initialization turns on cascading, sets the shouldCloseDocument property to false, and sets the autosave name for the window’s frame to an empty string.

## See Also

### Initializing Window Controllers

init(window: NSWindow?)

Returns a window controller initialized with a given window.

convenience init(windowNibName: NSNib.Name, owner: Any)

Returns a window controller initialized with a nib file and a specified owner for that nib file.

convenience init(windowNibPath: String, owner: Any)

Returns a window controller initialized with a nib file at an absolute path and a specified owner.

