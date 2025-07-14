

- HomeKit
- HMActionSet
-  updateName(\_:completionHandler:) 

Instance Method

# updateName(\_:completionHandler:)

Updates the name of the action set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateName(
    _ name: String,
    completionHandler completion: @escaping HMErrorBlock
)
```

``` source
func updateName(_ name: String) async throws
```

## Parameters 

`name`  

The new name; must not be `nil`.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Identifiying an action set

var uniqueIdentifier: UUID

The action set’s unique identifier.

var name: String

The name of the action set.

