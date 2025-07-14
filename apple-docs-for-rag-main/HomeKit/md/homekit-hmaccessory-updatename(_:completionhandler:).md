

- HomeKit
- HMAccessory
-  updateName(\_:completionHandler:) 

Instance Method

# updateName(\_:completionHandler:)

Changes the name of the accessory.

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

The new name.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Identifying an Accessory

var name: String

The name of the accessory.

var uniqueIdentifier: UUID

A unique identifier for the accessory.

var identifier: UUID

A unique identifier for the accessory.

Deprecated

