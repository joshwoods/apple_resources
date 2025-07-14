

- HomeKit
- HMServiceGroup
-  name 

Instance Property

# name

The name of the service group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Service group names must be unique within a home.

## See Also

### Related Documentation

HomeKit Developer Guide

### Managing Service Groups

var uniqueIdentifier: UUID

The unique identifier for the service group.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service group.

var services: [HMService]

Array of the services in the service group.

func addService(HMService, completionHandler: ((any Error)?) -> Void)

Adds a new service to the service group.

func removeService(HMService, completionHandler: ((any Error)?) -> Void)

Removes a service from the service group.

