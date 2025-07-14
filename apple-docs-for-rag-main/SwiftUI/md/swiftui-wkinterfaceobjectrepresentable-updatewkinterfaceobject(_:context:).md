

- SwiftUI
- WKInterfaceObjectRepresentable
-  updateWKInterfaceObject(\_:context:) 

Instance Method

# updateWKInterfaceObject(\_:context:)

Updates the presented WatchKit interface object (and its coordinator) to the latest configuration.

watchOS 6.0+

``` source
@MainActor @preconcurrency
func updateWKInterfaceObject(
    _ wkInterfaceObject: Self.WKInterfaceObjectType,
    context: Self.Context
)
```

**Required**

## Parameters 

`wkInterfaceObject`  

Your custom interface object.

`context`  

A context structure containing information about the current state of the system.

## Discussion

When the state of your app changes, SwiftUI updates the portions of your interface affected by those changes. SwiftUI calls this method for any changes affecting the corresponding interface object. Use this method to update the configuration of your object to match the new state information provided in the `context` parameter.

## See Also

### Creating and updating the interface object

func makeWKInterfaceObject(context: Self.Context) -> Self.WKInterfaceObjectType

Creates a WatchKit interface object and configures its initial state.

**Required**

typealias Context

