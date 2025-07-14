

- SwiftUI
- UIHostingController
-  init(coder:rootView:) 

Initializer

# init(coder:rootView:)

Creates a hosting controller object from an archive and the specified SwiftUI view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init?(
    coder aDecoder: NSCoder,
    rootView: Content
)
```

## Parameters 

`rootView`  

The root view of the SwiftUI view hierarchy that you want to manage using this view controller.

## Return Value

A `UIViewController` object that you can present from your interface.

## See Also

### Creating a hosting controller object

init(rootView: Content)

Creates a hosting controller object that wraps the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting controller object from the contents of the specified archive.

