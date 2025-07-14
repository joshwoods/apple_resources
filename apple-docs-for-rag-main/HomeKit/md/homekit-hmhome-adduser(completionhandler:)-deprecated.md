

- HomeKit
- HMHome
-  addUser(completionHandler:) Deprecated

Instance Method

# addUser(completionHandler:)

Adds a user to the home.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, visionOS**

``` source
func addUser(completionHandler completion: @escaping (HMUser?, (any Error)?) -> Void)
```

**visionOS**

``` source
func addUser() async throws -> HMUser
```

Deprecated

Use manageUsers(completionHandler:) instead.

## Parameters 

`completion`  

The block executed after the request is processed.

user  
The user that was added to the home.

error  
`nil` on success; otherwise, error object indicating the reason for failure. `error.userInfo[HMUserFailedAccessoriesKey]` contains more information in case of failure. See HMUserFailedAccessoriesKey for more details.

## See Also

### Deprecated symbols

var users: [HMUser]

All users associated with the home.

Deprecated

func removeUser(HMUser, completionHandler: ((any Error)?) -> Void)

Removes a user from the home.

Deprecated

