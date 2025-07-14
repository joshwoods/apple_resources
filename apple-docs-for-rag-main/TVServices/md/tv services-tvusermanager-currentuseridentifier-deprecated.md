

- TV Services
- TVUserManager
-  currentUserIdentifier Deprecated

Instance Property

# currentUserIdentifier

A unique identifier representing the currently active Apple TV user.

tvOS 13.0–16.0Deprecated

``` source
var currentUserIdentifier: TVUserIdentifier? { get }
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Discussion

Use this property to identify which Apple TV user is currently active. On Apple TV, users may provide credentials for multiple Apple accounts and switch quickly between them. This property uniquely identifies the user for the active account. You might use this information to select an appropriate user profile for your app.

The string in this property is randomly generated, and isn’t the same as the user’s Apple ID. Don’t display the string to your users. All Apple TVs on the user’s HomeKit network return the same string for the same account.

You can track changes to this property using key-value observing. You may access this property from an app extension.

## See Also

### Deprecated symbols

class let currentUserIdentifierDidChangeNotification: NSNotification.Name

The notification the system sends when a different user becomes current.

Deprecated

func presentProfilePreferencePanel(currentSettings: [TVUserIdentifier : TVAppProfileDescriptor], availableProfiles: [TVAppProfileDescriptor], completion: ([TVUserIdentifier : TVAppProfileDescriptor]) -> Void)

Presents a user-to-profile configuration panel, which lets the user specify their preferred profile.

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

