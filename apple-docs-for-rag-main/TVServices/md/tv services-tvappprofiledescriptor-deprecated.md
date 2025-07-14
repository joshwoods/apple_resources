

- TV Services
-  TVAppProfileDescriptor Deprecated

Class

# TVAppProfileDescriptor

A model object that you use to represent an app-specific profile.

tvOS 13.0–16.0Deprecated

``` source
class TVAppProfileDescriptor
```

Deprecated

Manually mapping profiles is deprecated. To opt-in to the system’s automatic user-data management, add the User Management Entitlement to your target, with a value of `runs-as-current-user-with-user-independent-keychain`. For more information, see Mapping Apple TV users to app profiles.

## Overview

A TVAppProfileDescriptor object represents a single user profile in your app. You create app profile descriptor objects yourself and manage them in your app’s data structures. The default object contains only the user-visible name for the profile, which must be a nonempty string. You can also subclass to add app-specific properties. For example, you might add an app-specific identifier for the profile. You might also store the identifiers for all Apple TV users that are configured to use this profile.

For more information about mapping your app profiles to Apple TV accounts, see TVUserManager.

## Topics

### Creating a Profile Descriptor

init(name: String)

Creates a new app profile descriptor object with the specified name.

### Getting the Profile Name

var name: String

The user-visible label associated with the app profile.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

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

typealias TVUserIdentifier

A unique string for differentiating between accounts on Apple TV.

Deprecated

var userIdentifiersForCurrentProfile: [TVUserIdentifier]

An array of system user identifiers that you associated with the current app-specific profile.

Deprecated

