

- AppKit
- NSWindowController
-  close() 

Instance Method

# close()

Closes the window if it was loaded.

macOS

``` source
@MainActor
func close()
```

## Discussion

Because this method closes the window without asking the user for confirmation, you usually do not invoke it when the Close menu command is chosen. Instead invoke NSWindow’s performClose(_:) on the receiver’s window.

## See Also

### Closing the Window

var shouldCloseDocument: Bool

A Boolean value that indicates whether the receiver necessarily closes the associated document when the window it manages is closed.

