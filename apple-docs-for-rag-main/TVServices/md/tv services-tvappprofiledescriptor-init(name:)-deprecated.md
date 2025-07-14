

- TV Services
- TVAppProfileDescriptor
-  init(name:) Deprecated

Initializer

# init(name:)

Creates a new app profile descriptor object with the specified name.

tvOS 13.0–16.0Deprecated

``` source
init(name: String)
```

Deprecated

User Management capability get-current-user is no longer supported. Please use runs-as-current-user-with-user-independent-keychain and kSecUseUserIndependentKeychain for sharing keychain items across users.

## Parameters 

`name`  

The user-visible string to display for the profile.

## Return Value

An initialized app profile descriptor object.

