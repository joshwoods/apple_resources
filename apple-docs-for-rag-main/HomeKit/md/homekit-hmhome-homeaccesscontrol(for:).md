

- HomeKit
- HMHome
-  homeAccessControl(for:) 

Instance Method

# homeAccessControl(for:)

Retrieves the access level of a user associated with the home.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func homeAccessControl(for user: HMUser) -> HMHomeAccessControl
```

## Parameters 

`user`  

The user whose access level you wish to retrieve.

## Return Value

The access level associated with the user.

## See Also

### Controlling user access

class HMHomeAccessControl

The access privileges of a user associated with a home.

class HMAccessControl

An abstract superclass for accessing user privileges.

let HMUserFailedAccessoriesKey: String

The key for retrieving details of what accessories failed to add or remove a user.

