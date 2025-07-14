

- HomeKit
- HMHome
-  manageUsers(completionHandler:) 

Instance Method

# manageUsers(completionHandler:)

Presents a view controller to manage users of the home.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
func manageUsers(completionHandler completion: @escaping ((any Error)?) -> Void)
```

``` source
func manageUsers() async throws
```

## Parameters 

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

Only users that have administrator access to the home can call this method. Otherwise, the completion handler returns the error HMError.Code.insufficientPrivileges.

## See Also

### Managing users

var currentUser: HMUser

The current HomeKit user.

class HMUser

A person in the home who may have access to control accessories and services in the home.

