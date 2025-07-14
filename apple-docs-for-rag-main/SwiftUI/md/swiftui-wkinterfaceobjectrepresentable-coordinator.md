

- SwiftUI
- WKInterfaceObjectRepresentable
-  Coordinator 

Associated Type

# Coordinator

A type to coordinate with the WatchKit interface object.

watchOS 6.0+

``` source
associatedtype Coordinator = Void
```

**Required**

## See Also

### Providing a custom coordinator object

func makeCoordinator() -> Self.Coordinator

Creates the custom instance that you use to communicate changes from your interface object to other parts of your SwiftUI interface.

**Required** Default implementation provided.

associatedtype WKInterfaceObjectType : WKInterfaceObject

The type of WatchKit interface object to be presented.

**Required**

