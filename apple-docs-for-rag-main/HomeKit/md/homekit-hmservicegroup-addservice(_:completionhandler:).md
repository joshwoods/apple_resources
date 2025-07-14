

- HomeKit
- HMServiceGroup
-  addService(\_:completionHandler:) 

Instance Method

# addService(\_:completionHandler:)

Adds a new service to the service group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func addService(
    _ service: HMService,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func addService(_ service: HMService) async throws
```

## Parameters 

`service`  

The service to add.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

A service can be added to multiple service groups. For example, a light could be added to the “Desk Lamps” service group as well as the “Dimmable Lights” service group.

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

func removeService(HMService, completionHandler: ((any Error)?) -> Void)

Removes a service from the service group.

