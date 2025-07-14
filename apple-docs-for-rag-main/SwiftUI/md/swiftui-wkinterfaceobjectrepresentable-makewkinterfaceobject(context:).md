

- SwiftUI
- WKInterfaceObjectRepresentable
-  makeWKInterfaceObject(context:) 

Instance Method

# makeWKInterfaceObject(context:)

Creates a WatchKit interface object and configures its initial state.

watchOS 6.0+

``` source
@MainActor @preconcurrency
func makeWKInterfaceObject(context: Self.Context) -> Self.WKInterfaceObjectType
```

**Required**

## Parameters 

`context`  

A context structure containing information about the current state of the system.

## Return Value

Your interface object configured with the provided information.

## Discussion

You must implement this method and use it to create your interface object. Configure the object using your app’s current data and contents of the `context` parameter. The system calls this method only once, when it creates your interface object for the first time. For all subsequent updates, the system calls the updateWKInterfaceObject(_:context:) method.

## See Also

### Creating and updating the interface object

func updateWKInterfaceObject(Self.WKInterfaceObjectType, context: Self.Context)

Updates the presented WatchKit interface object (and its coordinator) to the latest configuration.

**Required**

typealias Context

