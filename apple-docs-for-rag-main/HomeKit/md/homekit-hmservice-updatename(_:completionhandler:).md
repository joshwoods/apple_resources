

- HomeKit
- HMService
-  updateName(\_:completionHandler:) 

Instance Method

# updateName(\_:completionHandler:)

Updates the name of the service to the specified string.

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

The new name. Must not match an existing name in the home.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Identifying the service

var name: String

The user specified name of the service.

var uniqueIdentifier: UUID

A unique identifier for the service.

