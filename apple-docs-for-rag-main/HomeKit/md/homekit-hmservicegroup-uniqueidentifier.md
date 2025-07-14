

- HomeKit
- HMServiceGroup
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

The unique identifier for the service group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifier: UUID { get }
```

## See Also

### Managing Service Groups

var name: String

The name of the service group.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service group.

var services: [HMService]

Array of the services in the service group.

func addService(HMService, completionHandler: ((any Error)?) -> Void)

Adds a new service to the service group.

func removeService(HMService, completionHandler: ((any Error)?) -> Void)

Removes a service from the service group.

