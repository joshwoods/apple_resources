

- StoreKit
- SKCloudServiceController
-  Requesting Access to Apple Music Library 

Article

# Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

## Overview

Your app must obtain permission from the customer before accessing Apple Music Library.

### Provide a Purpose String in Info.plist

Provide a purpose string or usage description that describes how your app intends to use the user’s iCloud Music library or Apple Music catalog. Add the NSAppleMusicUsageDescription key to your app’s Info.plist. Set its value to a string that explains why your app needs access to Apple Music library. The system displays the string to the user when prompting them for authorization.

Important

This key is required for apps that access the user’s music library. Apps crash when the key is absent.

See Requesting access to protected resources for more details.

### Request Authorization

The user determines whether apps can play items from the Apple Music catalog or add tracks to their iCloud Music library. They can grant or deny access when your app requests authorization. Because the user can change your app’s authorization status in Settings \> Privacy \> Media and Apple Music, be sure to call SKCloudServiceController’s authorizationStatus() before attempting to access their Apple Music library.

- Swift
- Objective-C

```
guard SKCloudServiceController.authorizationStatus() == .notDetermined else { return }
```

```
SKCloudServiceAuthorizationStatus status = ([SKCloudServiceController authorizationStatus] == SKCloudServiceAuthorizationStatusNotDetermined);
```

If the authorization status i`s` SKCloudServiceAuthorizationStatus.notDetermined, call SKCloudServiceController’s requestAuthorization(_:) to prompt the user for access.

- Swift
- Objective-C

```
SKCloudServiceController.requestAuthorization {(status: SKCloudServiceAuthorizationStatus) in
    switch status {
    case .denied, .restricted: disableAppleMusicBasedFeatures()
    case .authorized: enableAppleMusicBasedFeatures()
    default: break
    }
}
```

```
[SKCloudServiceController requestAuthorization:^(SKCloudServiceAuthorizationStatus status) {
    switch (status) {
        case SKCloudServiceAuthorizationStatusDenied:
        case SKCloudServiceAuthorizationStatusRestricted: [self disableAppleMusicBasedFeatures];
            break;
        case SKCloudServiceAuthorizationStatusAuthorized: [self enableAppleMusicBasedFeatures];
            break;
        default: break;
    }
}];

```

The system remembers the user’s answer so that subsequent calls to requestAuthorization(_:) don’t prompt them again.

## See Also

### Getting authorization to access the Music library

class func authorizationStatus() -> SKCloudServiceAuthorizationStatus

Returns the type of authorization the customer has for accessing the Music library on the device.

Deprecated

class func requestAuthorization((SKCloudServiceAuthorizationStatus) -> Void)

Asks the customer for permission to access the Music library on the device.

Deprecated

enum SKCloudServiceAuthorizationStatus

Constants that indicate the type of authorization the customer has for accessing the Music library.

Deprecated

