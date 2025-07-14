

- SwiftUI
- WKInterfaceObjectRepresentable
-  WKInterfaceObjectRepresentable.Context 

Type Alias

# WKInterfaceObjectRepresentable.Context

watchOS 6.0+

``` source
typealias Context = WKInterfaceObjectRepresentableContext
```

## See Also

### Creating and updating the interface object

func makeWKInterfaceObject(context: Self.Context) -> Self.WKInterfaceObjectType

Creates a WatchKit interface object and configures its initial state.

**Required**

func updateWKInterfaceObject(Self.WKInterfaceObjectType, context: Self.Context)

Updates the presented WatchKit interface object (and its coordinator) to the latest configuration.

**Required**

