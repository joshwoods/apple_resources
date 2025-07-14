

- SwiftUI
- NSHostingController
-  init(coder:) 

Initializer

# init(coder:)

Creates a hosting controller object from the contents of the specified archive.

macOS 10.15+

``` source
@MainActor @preconcurrency
required dynamic init?(coder: NSCoder)
```

## Parameters 

`coder`  

The decoder to use during initialization.

## Discussion

The default implementation of this method throws an exception. To create your view controller from an archive, override this method and initialize the superclass using the init(coder:rootView:) method instead.

## See Also

### Creating a hosting controller object

init(rootView: Content)

Creates a hosting controller object that wraps the specified SwiftUI view.

init?(coder: NSCoder, rootView: Content)

Creates a hosting controller object from an archive and the specified SwiftUI view.

