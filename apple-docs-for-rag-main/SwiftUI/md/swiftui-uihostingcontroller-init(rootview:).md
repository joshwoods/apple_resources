

- SwiftUI
- UIHostingController
-  init(rootView:) 

Initializer

# init(rootView:)

Creates a hosting controller object that wraps the specified SwiftUI view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(rootView: Content)
```

## Parameters 

`rootView`  

The root view of the SwiftUI view hierarchy that you want to manage using the hosting view controller.

## Return Value

A `UIHostingController` object initialized with the specified SwiftUI view.

## See Also

### Creating a hosting controller object

init?(coder: NSCoder, rootView: Content)

Creates a hosting controller object from an archive and the specified SwiftUI view.

init?(coder: NSCoder)

Creates a hosting controller object from the contents of the specified archive.

