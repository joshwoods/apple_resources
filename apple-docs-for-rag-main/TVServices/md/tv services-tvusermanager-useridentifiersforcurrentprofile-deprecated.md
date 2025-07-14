

- TV Services
- TVUserManager
-  userIdentifiersForCurrentProfile Deprecated

Instance Property

# userIdentifiersForCurrentProfile

An array of system user identifiers that you associated with the current app-specific profile.

tvOS 13.0–16.0Deprecated

``` source
var userIdentifiersForCurrentProfile: [TVUserIdentifier] { get set }
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Discussion

If your app remembers which app-specific profile each Apple TV user prefers, use this property to provide that information to the system. Fill this property with zero or more user identifiers that you previously retrieved from the currentUserIdentifier property. Doing so creates a mapping between your app profiles and the Apple TV accounts that prefer them. The system uses the information in this property to provide better information in user dialogs and doesn’t change the property’s value.

Update this property whenever the user selects a different app profile. The system doesn’t change the value in this property, so it contains the last value that you assigned to it since app launch. However, the property supports key-value observing if you want to track the changes that you make from other parts of your app.

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

func shouldStorePreferenceForCurrentUser(to: TVAppProfileDescriptor, completion: (Bool) -> Void)

Prompts the user to save the specified profile as the preferred profile for the current user.

Deprecated

class TVAppProfileDescriptor

A model object that you use to represent an app-specific profile.

Deprecated

typealias TVUserIdentifier

A unique string for differentiating between accounts on Apple TV.

Deprecated

