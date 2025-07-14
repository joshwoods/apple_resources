

- HomeKit
- HMHome
-  removeUser(\_:completionHandler:) Deprecated

Instance Method

# removeUser(\_:completionHandler:)

Removes a user from the home.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func removeUser(
    _ user: HMUser,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

**Mac Catalyst, visionOS**

``` source
func removeUser(_ user: HMUser) async throws
```

Deprecated

Use manageUsers(completionHandler:) instead.

## Parameters 

`user`  

The user to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure. `error.userInfo[HMUserFailedAccessoriesKey]` contains more information in case of failure. See HMUserFailedAccessoriesKey for more details.

## See Also

### Deprecated symbols

var users: [HMUser]

All users associated with the home.

Deprecated

func addUser(completionHandler: (HMUser?, (any Error)?) -> Void)

Adds a user to the home.

Deprecated

