

- SwiftUI
- NSHostingView
-  init(coder:rootView:) 

Initializer

# init(coder:rootView:)

Creates a hosting view object from an archive and the specified SwiftUI view.

macOS 15.4+

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

The root view of the SwiftUI view hierarchy that you want to manage using this hosting view.

