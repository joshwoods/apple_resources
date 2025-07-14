

- SwiftUI
- NSViewRepresentable
-  makeCoordinator() 

Instance Method

# makeCoordinator()

Creates the custom instance that you use to communicate changes from your view to other parts of your SwiftUI interface.

macOS 10.15+

``` source
@MainActor @preconcurrency
func makeCoordinator() -> Self.Coordinator
```

**Required** Default implementation provided.

## Discussion

Implement this method if changes to your view might affect other parts of your app. In your implementation, create a custom Swift instance that can communicate with other parts of your interface. For example, you might provide an instance that binds its variables to SwiftUI properties, causing the two to remain synchronized. If your view doesn’t interact with other parts of your app, you don’t have to provide a coordinator.

SwiftUI calls this method before calling the makeNSView(context:) method. The system provides your coordinator instance either directly or as part of a context structure when calling the other methods of your representable instance.

## Default Implementations

### NSViewRepresentable Implementations

func makeCoordinator() -> Self.Coordinator

Creates a `Coordinator` instance to coordinate with the `NSView`.

## See Also

### Providing a custom coordinator object

associatedtype Coordinator = Void

A type to coordinate with the view.

**Required**

