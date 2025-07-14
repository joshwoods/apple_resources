

- SwiftUI
- WKInterfaceObjectRepresentable
-  makeCoordinator() 

Instance Method

# makeCoordinator()

Creates the custom instance that you use to communicate changes from your interface object to other parts of your SwiftUI interface.

watchOS 6.0+

``` source
@MainActor @preconcurrency
func makeCoordinator() -> Self.Coordinator
```

**Required** Default implementation provided.

## Discussion

Implement this method if changes to your interface object might affect other parts of your app. In your implementation, create a custom Swift instance that can communicate with other parts of your interface. For example, you might provide an instance that binds its variables to SwiftUI properties, causing the two to remain synchronized. If your interface object doesn’t interact with other parts of your app, providing a coordinator is unnecessary.

SwiftUI calls this method before calling the makeWKInterfaceObject(context:) method. The system provides your coordinator either directly or as part of a context structure when calling the other methods of your representable instance.

## Default Implementations

### WKInterfaceObjectRepresentable Implementations

func makeCoordinator() -> Self.Coordinator

Creates the custom instance that you use to communicate changes from your interface object to other parts of your SwiftUI interface.

## See Also

### Providing a custom coordinator object

associatedtype Coordinator = Void

A type to coordinate with the WatchKit interface object.

**Required**

associatedtype WKInterfaceObjectType : WKInterfaceObject

The type of WatchKit interface object to be presented.

**Required**

