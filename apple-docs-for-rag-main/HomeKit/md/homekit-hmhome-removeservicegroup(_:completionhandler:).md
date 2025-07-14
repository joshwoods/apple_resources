

- HomeKit
- HMHome
-  removeServiceGroup(\_:completionHandler:) 

Instance Method

# removeServiceGroup(\_:completionHandler:)

Removes a service group from the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func removeServiceGroup(
    _ group: HMServiceGroup,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeServiceGroup(_ group: HMServiceGroup) async throws
```

## Parameters 

`group`  

The service group to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Grouping services

func servicesWithTypes([String]) -> [HMService]?

Returns an array of all services provided by accessories in the home that match the specified types.

var serviceGroups: [HMServiceGroup]

An array of all service groups in the home.

func addServiceGroup(withName: String, completionHandler: (HMServiceGroup?, (any Error)?) -> Void)

Adds a service group to the home.

class HMServiceGroup

A collection of accessory services.

