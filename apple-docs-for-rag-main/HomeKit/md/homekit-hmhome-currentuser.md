

- HomeKit
- HMHome
-  currentUser 

Instance Property

# currentUser

The current HomeKit user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currentUser: HMUser { get }
```

## See Also

### Managing users

func manageUsers(completionHandler: ((any Error)?) -> Void)

Presents a view controller to manage users of the home.

class HMUser

A person in the home who may have access to control accessories and services in the home.

