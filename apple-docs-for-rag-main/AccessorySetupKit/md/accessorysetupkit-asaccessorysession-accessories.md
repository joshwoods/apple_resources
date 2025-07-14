

- AccessorySetupKit
- ASAccessorySession
-  accessories 

Instance Property

# accessories

An array of previously-selected accessories for this application.

iOS 18.0+iPadOS 18.0+

``` source
var accessories: [ASAccessory] { get }
```

## Mentioned in 

Discovering and configuring accessories

## Discussion

To monitor for changes in this list, use your event handler to watch for the events ASAccessoryEventType.accessoryAdded, ASAccessoryEventType.accessoryChanged, and ASAccessoryEventType.accessoryRemoved.

