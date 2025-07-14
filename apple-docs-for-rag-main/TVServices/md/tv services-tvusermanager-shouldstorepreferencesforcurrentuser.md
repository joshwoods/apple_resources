

- TV Services
- TVUserManager
-  shouldStorePreferencesForCurrentUser 

Instance Property

# shouldStorePreferencesForCurrentUser

A Boolean value that indicates whether your app needs to retain a selected profile.

tvOS 16.0+

``` source
var shouldStorePreferencesForCurrentUser: Bool { get }
```

## Discussion

Important

To create a TVUserManager object, add the User Management Entitlement to your app or app extension, and select the Runs as Current User, Only When User-Independent Keychain is Available option.

Some apps rely on profiles to maintain separate information for each person who uses a shared device, such as a video content app that retains which shows they watch. To avoid interrupting people with a profile picker each time they launch your app, you can save the current user’s selection on a shared device. After someone selects a profile, use shouldStorePreferencesForCurrentUser to determine whether to retain the profile selection or to prompt each time your app launches. This property might be false if people share a device, but don’t configure multiple users on that device.

If the property’s value is false, display the profile picker to determine which profile to use for the current session, but don’t save the selected profile. If the value is true, and there isn’t a saved profile in UserDefaults, display the profile picker and save the selected profile for future use. If the value is true and there’s already a saved profile, skip the prompt and use the saved profile.

Tip

When your app runs in tvOS 15 or earlier, where shouldStorePreferencesForCurrentUser isn’t available, display the profile picker at the beginning of each session.

