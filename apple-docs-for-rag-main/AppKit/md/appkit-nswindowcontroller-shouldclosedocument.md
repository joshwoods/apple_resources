

- AppKit
- NSWindowController
-  shouldCloseDocument 

Instance Property

# shouldCloseDocument

A Boolean value that indicates whether the receiver necessarily closes the associated document when the window it manages is closed.

macOS

``` source
@MainActor
var shouldCloseDocument: Bool { get set }
```

## Discussion

The value of this property is true if the receiver necessarily closes the associated document when the window it manages is closed, false otherwise. The default value is false.

## See Also

### Closing the Window

func close()

Closes the window if it was loaded.

