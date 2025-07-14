

- SwiftUI
- NSViewRepresentable
-  Coordinator 

Associated Type

# Coordinator

A type to coordinate with the view.

macOS 10.15+

``` source
associatedtype Coordinator = Void
```

**Required**

## See Also

### Providing a custom coordinator object

func makeCoordinator() -> Self.Coordinator

Creates the custom instance that you use to communicate changes from your view to other parts of your SwiftUI interface.

**Required** Default implementation provided.

