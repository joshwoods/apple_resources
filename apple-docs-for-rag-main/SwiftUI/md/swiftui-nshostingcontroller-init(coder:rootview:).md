

- SwiftUI
- NSHostingController
-  init(coder:rootView:) 

Initializer

# init(coder:rootView:)

Creates a hosting controller object from an archive and the specified SwiftUI view.

macOS 10.15+

``` source
@MainActor @preconcurrency
init?(
    coder: NSCoder,
    rootView: Content
)
```

## Parameters 

`coder`  

The decoder to use during initialization.

`rootView`  

The root view of the SwiftUI view hierarchy that you want to manage using this view controller.

## See Also

### Creating a hosting controller object

init(rootView: Content)

Creates a hosting controller object that wraps the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting controller object from the contents of the specified archive.

