

- SwiftUI
- WKInterfaceObjectRepresentable
-  dismantleWKInterfaceObject(\_:coordinator:) 

Type Method

# dismantleWKInterfaceObject(\_:coordinator:)

Cleans up the presented WatchKit interface object (and its coordinator) in anticipation of their removal.

watchOS 6.0+

``` source
@MainActor @preconcurrency
static func dismantleWKInterfaceObject(
    _ wkInterfaceObject: Self.WKInterfaceObjectType,
    coordinator: Self.Coordinator
)
```

**Required** Default implementation provided.

## Parameters 

`wkInterfaceObject`  

Your custom interface object.

`coordinator`  

The custom coordinator instance you use to communicate changes back to SwiftUI. If you do not use a custom coordinator, the system provides a default instance.

## Discussion

Use this method to perform additional clean-up work related to your custom interface object. For example, you might use this method to remove observers or update other parts of your SwiftUI interface.

## Default Implementations

### WKInterfaceObjectRepresentable Implementations

static func dismantleWKInterfaceObject(Self.WKInterfaceObjectType, coordinator: Self.Coordinator)

Cleans up the presented interface object (and coordinator) in anticipation of their removal.

