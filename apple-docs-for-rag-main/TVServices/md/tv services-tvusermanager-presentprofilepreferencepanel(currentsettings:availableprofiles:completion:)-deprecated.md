

- TV Services
- TVUserManager
-  presentProfilePreferencePanel(currentSettings:availableProfiles:completion:) Deprecated

Instance Method

# presentProfilePreferencePanel(currentSettings:availableProfiles:completion:)

Presents a user-to-profile configuration panel, which lets the user specify their preferred profile.

tvOS 13.0–16.0Deprecated

``` source
func presentProfilePreferencePanel(
    currentSettings: [TVUserIdentifier : TVAppProfileDescriptor],
    availableProfiles: [TVAppProfileDescriptor],
    completion: @escaping ([TVUserIdentifier : TVAppProfileDescriptor]) -> Void
)
```

``` source
func presentProfilePreferencePanel(
    currentSettings: [TVUserIdentifier : TVAppProfileDescriptor],
    availableProfiles: [TVAppProfileDescriptor]
) async -> [TVUserIdentifier : TVAppProfileDescriptor]
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Parameters 

`availableProfiles`  

The complete list of app-specific profiles available in your app. The configuration panel displays this set of profiles to the user.

`completion`  

The completion handler to call when the user dismisses the configuration panel. This handler has no return value and takes the following parameter:

newSettings  
A dictionary containing an updated map from system user to app profile. The information is similar to what you provide in the `existingSettings` parameter, but reflects the changes made by the user.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func presentProfilePreferencePanel(currentSettings: [TVUserIdentifier : TVAppProfileDescriptor], availableProfiles: [TVAppProfileDescriptor]) async -> [TVUserIdentifier : TVAppProfileDescriptor]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Calling this method displays a panel that lets the user configure which app-specific profile to associate with each Apple TV user account. The panel gives the user the option to select from any of the profiles in the `availableProfiles` parameter. It also uses the information in the `existingSettings` parameter to configure the initial mapping between users and profiles. After configuring the user accounts and dismissing the panel, the system calls your `completion` handler to deliver the updated mapping between user accounts and profiles.

## See Also

### Deprecated symbols

var currentUserIdentifier: TVUserIdentifier?

A unique identifier representing the currently active Apple TV user.

Deprecated

class let currentUserIdentifierDidChangeNotification: NSNotification.Name

The notification the system sends when a different user becomes current.

Deprecated

func shouldStorePreferenceForCurrentUser(to: TVAppProfileDescriptor, completion: (Bool) -> Void)

Prompts the user to save the specified profile as the preferred profile for the current user.

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

