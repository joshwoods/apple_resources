

- HomeKit
- HMServiceGroup
-  removeService(\_:completionHandler:) 

Instance Method

# removeService(\_:completionHandler:)

Removes a service from the service group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func removeService(
    _ service: HMService,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeService(_ service: HMService) async throws
```

## Parameters 

`service`  

The service to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Managing Service Groups

var name: String

The name of the service group.

var uniqueIdentifier: UUID

The unique identifier for the service group.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service group.

var services: [HMService]

Array of the services in the service group.

func addService(HMService, completionHandler: ((any Error)?) -> Void)

Adds a new service to the service group.

