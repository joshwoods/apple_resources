

- HomeKit
- HMHome
-  servicesWithTypes(\_:) 

Instance Method

# servicesWithTypes(\_:)

Returns an array of all services provided by accessories in the home that match the specified types.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func servicesWithTypes(_ serviceTypes: [String]) -> [HMService]?
```

## Parameters 

`serviceTypes`  

An array of strings that identify service types. See Accessory Service Types for a list of types.

## Return Value

An array of found services. Returns `nil` if no matching services are found.

## See Also

### Grouping services

var serviceGroups: [HMServiceGroup]

An array of all service groups in the home.

func addServiceGroup(withName: String, completionHandler: (HMServiceGroup?, (any Error)?) -> Void)

Adds a service group to the home.

func removeServiceGroup(HMServiceGroup, completionHandler: ((any Error)?) -> Void)

Removes a service group from the home.

class HMServiceGroup

A collection of accessory services.

