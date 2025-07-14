

- SwiftUI
- NSHostingView
-  init(coder:) 

Initializer

# init(coder:)

Creates a hosting view object from the contents of the specified archive.

macOS 10.15+

``` source
@MainActor @preconcurrency
required dynamic init?(coder aDecoder: NSCoder)
```

## Discussion

The default implementation of this method throws an exception. To create your view from an archive, override this method and initialize the superclass using the init(coder:rootView:) method instead.

## See Also

### Creating a hosting view

init(rootView: Content)

Creates a hosting view object that wraps the specified SwiftUI view.

func prepareForReuse()

