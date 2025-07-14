

- SwiftUI
- UIViewControllerRepresentable
-  Coordinator 

Associated Type

# Coordinator

A type to coordinate with the view controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
associatedtype Coordinator = Void
```

**Required**

## See Also

### Providing a custom coordinator object

func makeCoordinator() -> Self.Coordinator

Creates the custom instance that you use to communicate changes from your view controller to other parts of your SwiftUI interface.

**Required** Default implementation provided.

