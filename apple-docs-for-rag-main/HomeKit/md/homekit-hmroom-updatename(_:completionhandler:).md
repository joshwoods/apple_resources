

- HomeKit
- HMRoom
-  updateName(\_:completionHandler:) 

Instance Method

# updateName(\_:completionHandler:)

Updates the name of the room.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateName(
    _ name: String,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateName(_ name: String) async throws
```

## Parameters 

`name`  

The new name which must not be `nil`.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Identifying a room

var name: String

The name of the room.

var uniqueIdentifier: UUID

The unique identifier for a room.

