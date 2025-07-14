

- HomeKit
- HMHome
-  updateName(\_:completionHandler:) 

Instance Method

# updateName(\_:completionHandler:)

Updates the name of the home.

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

The new name. Must not already exist in the home.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Identifying a home

var name: String

The name the user gives to the home.

var uniqueIdentifier: UUID

A unique identifier for the home.

var isPrimary: Bool

A Boolean value that indicates whether this is the primary home for its home manager.

