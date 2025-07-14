

- HomeKit
- HMHome
-  serviceGroups 

Instance Property

# serviceGroups

An array of all service groups in the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var serviceGroups: [HMServiceGroup] { get }
```

## Discussion

Services groups are instances of HMServiceGroup.

## See Also

### Grouping services

func servicesWithTypes([String]) -> [HMService]?

Returns an array of all services provided by accessories in the home that match the specified types.

func addServiceGroup(withName: String, completionHandler: (HMServiceGroup?, (any Error)?) -> Void)

Adds a service group to the home.

func removeServiceGroup(HMServiceGroup, completionHandler: ((any Error)?) -> Void)

Removes a service group from the home.

class HMServiceGroup

A collection of accessory services.

