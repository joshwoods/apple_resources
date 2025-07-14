

- HomeKit
-  HMUserFailedAccessoriesKey 

Global Variable

# HMUserFailedAccessoriesKey

The key for retrieving details of what accessories failed to add or remove a user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMUserFailedAccessoriesKey: String
```

## Discussion

The value associated with this key is an NSArray of NSDictionary objects. Each dictionary contains the UUID of the accessory that failed to be added/removed and the value corresponding to the dictionary key is an NSError that provides more details on the underlying error for that accessory.

## See Also

### Controlling user access

func homeAccessControl(for: HMUser) -> HMHomeAccessControl

Retrieves the access level of a user associated with the home.

class HMHomeAccessControl

The access privileges of a user associated with a home.

class HMAccessControl

An abstract superclass for accessing user privileges.

