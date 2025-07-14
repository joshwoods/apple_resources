

- AppKit
- NSDocumentController
-  init() 

Initializer

# init()

This method is the designated initializer for `NSDocumentController`.

macOS

``` source
@MainActor
init()
```

## Return Value

The initialized document controller object.

## Discussion

The first instance of `NSDocumentController` or any of its subclasses that is created becomes the shared instance.

## See Also

### Initializing a New NSDocumentController

init?(coder: NSCoder)

This method initializes a new NSDocumentController from the coder.

