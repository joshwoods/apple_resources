

- HomeKit
- HMRoom
-  name 

Instance Property

# name

The name of the room.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Allow the user to choose room names. Room names must be unique within a home.

## See Also

### Identifying a room

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the room.

var uniqueIdentifier: UUID

The unique identifier for a room.

