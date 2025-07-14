

- HomeKit
- HMHome
-  addServiceGroup(withName:completionHandler:) 

Instance Method

# addServiceGroup(withName:completionHandler:)

Adds a service group to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addServiceGroup(
    withName serviceGroupName: String,
    completionHandler completion: @escaping (HMServiceGroup?, (any Error)?) -> Void
)
```

``` source
func addServiceGroup(named serviceGroupName: String) async throws -> HMServiceGroup
```

## Parameters 

`serviceGroupName`  

The name of the new service group. Must not be `nil`, and must not be the name of a service group already in the home.

`completion`  

The block executed after the request is processed.

group  
The newly created service group.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Grouping services

func servicesWithTypes([String]) -> [HMService]?

Returns an array of all services provided by accessories in the home that match the specified types.

var serviceGroups: [HMServiceGroup]

An array of all service groups in the home.

func removeServiceGroup(HMServiceGroup, completionHandler: ((any Error)?) -> Void)

Removes a service group from the home.

class HMServiceGroup

A collection of accessory services.

