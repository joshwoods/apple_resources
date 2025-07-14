

- SwiftUI
- NSViewControllerRepresentable
-  Coordinator 

Associated Type

# Coordinator

A type to coordinate with the view controller.

macOS 10.15+

``` source
associatedtype Coordinator = Void
```

**Required**

## See Also

### Providing a custom coordinator object

func makeCoordinator() -> Self.Coordinator

Creates the custom object that you use to communicate changes from your view controller to other parts of your SwiftUI interface.

**Required** Default implementation provided.

