

- TV Services
- TVUserManager
-  currentUserIdentifierDidChangeNotification Deprecated

Type Property

# currentUserIdentifierDidChangeNotification

The notification the system sends when a different user becomes current.

tvOS 13.0–16.0Deprecated

``` source
class let currentUserIdentifierDidChangeNotification: NSNotification.Name
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Discussion

The object of the notification is `nil`. The notification doesn’t add any keys to the userInfo dictionary.

## See Also

### Deprecated symbols

var currentUserIdentifier: TVUserIdentifier?

A unique identifier representing the currently active Apple TV user.

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

