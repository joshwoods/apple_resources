

- TV Services
-  TVUserManager 

Class

# TVUserManager

An object that indicates how to store preferences for multiple people on a shared device.

tvOS 13.0+

``` source
class TVUserManager
```

## Overview

Some apps rely on profiles to maintain separate information for each person who uses a shared device, such as a video content app that retains which shows they watch. To avoid interrupting people with a profile picker each time they launch your app, you can save and retrieve the current user’s selection on a shared device.

Important

To create a TVUserManager object, add the User Management Entitlement capability to your app or app extension in Xcode, and select the Runs as Current User, Only When User-Independent Keychain is Available option. This enables the system to take care of separating each user’s data for your app.

To determine the current user’s profile, first check shouldStorePreferencesForCurrentUser. If that value is false, display the profile picker to determine which profile to use for the current session, but don’t save the selected profile. If the value is true, and there isn’t a saved profile in UserDefaults, display the profile picker and save the selected profile for future use. If the value is true and there’s already a saved profile, skip the prompt and use the saved profile.

## Topics

### Retaining profile selection for the current Apple TV account

var shouldStorePreferencesForCurrentUser: Bool

A Boolean value that indicates whether your app needs to retain a selected profile.

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

var userIdentifiersForCurrentProfile: [TVUserIdentifier]

An array of system user identifiers that you associated with the current app-specific profile.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Multiple users

Personalizing Your App for Each User on Apple TV

Use account-specific storage to segregate data on a multiuser system.

Supporting Multiple Users in Your tvOS App

Store separate data for each user with the new Runs as Current User capability.

Mapping Apple TV users to app profiles

Adapt the content of your app for the current viewer by using an entitlement and simplifying sign-in flows.

