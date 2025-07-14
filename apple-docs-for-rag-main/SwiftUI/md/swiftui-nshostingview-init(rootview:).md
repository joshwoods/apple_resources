

- SwiftUI
- NSHostingView
-  init(rootView:) 

Initializer

# init(rootView:)

Creates a hosting view object that wraps the specified SwiftUI view.

macOS 10.15+

``` source
@MainActor @preconcurrency
required init(rootView: Content)
```

## Parameters 

`rootView`  

The root view of the SwiftUI view hierarchy that you want to manage using this hosting view.

## See Also

### Creating a hosting view

init?(coder: NSCoder)

Creates a hosting view object from the contents of the specified archive.

func prepareForReuse()

