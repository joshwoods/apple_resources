

- TV Services
- TVAppProfileDescriptor
-  name Deprecated

Instance Property

# name

The user-visible label associated with the app profile.

tvOS 13.0–16.0Deprecated

``` source
var name: String { get set }
```

Deprecated

User Management capability get-current-user is no longer supported. Please use runs-as-current-user-with-user-independent-keychain and kSecUseUserIndependentKeychain for sharing keychain items across users.

## Discussion

Use this property to store the user-readable name for the user profile. When prompting the user to select a preferred profile, the TVUserManager displays the names from your TVAppProfileDescriptor objects in the selection dialog.

You must specify a nonempty string in this property.

