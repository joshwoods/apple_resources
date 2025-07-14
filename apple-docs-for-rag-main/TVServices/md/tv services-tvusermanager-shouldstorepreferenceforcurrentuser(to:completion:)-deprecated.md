

- TV Services
- TVUserManager
-  shouldStorePreferenceForCurrentUser(to:completion:) Deprecated

Instance Method

# shouldStorePreferenceForCurrentUser(to:completion:)

Prompts the user to save the specified profile as the preferred profile for the current user.

tvOS 13.0–16.0Deprecated

``` source
func shouldStorePreferenceForCurrentUser(
    to profile: TVAppProfileDescriptor,
    completion: @escaping (Bool) -> Void
)
```

``` source
func shouldStorePreferenceForCurrentUser(to profile: TVAppProfileDescriptor) async -> Bool
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Parameters 

`profile`  

The profile to associate with the current user.

`completion`  

The completion handler to call with the results. This handler has no return value and takes the following parameter:

shouldCreateMapping  
A Boolean value indicating whether your app should associate the specified profile with the current user. If this parameter is true, save the association in your app’s data structures.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func shouldStorePreferenceForCurrentUser(to profile: TVAppProfileDescriptor) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to confirm that the profile chosen by the user should become their new preferred profile. The method prompts the user to confirm the profile change and calls the completion handler with the results. Call this method only once for each user.

## See Also

### Deprecated symbols

var currentUserIdentifier: TVUserIdentifier?

A unique identifier representing the currently active Apple TV user.

Deprecated

class let currentUserIdentifierDidChangeNotification: NSNotification.Name

The notification the system sends when a different user becomes current.

Deprecated

func presentProfilePreferencePanel(currentSettings: [TVUserIdentifier : TVAppProfileDescriptor], availableProfiles: [TVAppProfileDescriptor], completion: ([TVUserIdentifier : TVAppProfileDescriptor]) -> Void)

Presents a user-to-profile configuration panel, which lets the user specify their preferred profile.

Deprecated

class TVAppProfileDescriptor

A model object that you use to represent an app-specific profile.

Deprecated

typealias TVUserIdentifier

A unique string for differentiating between accounts on Apple TV.

Deprecated

var userIdentifiersForCurrentProfile: [TVUserIdentifier]

An array of system user identifiers that you associated with the current app-specific profile.

Deprecated

