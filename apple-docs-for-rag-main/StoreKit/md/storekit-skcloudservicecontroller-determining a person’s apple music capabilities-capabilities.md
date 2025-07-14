

- StoreKit
- SKCloudServiceController
-  Determining a person’s Apple Music capabilities 

Article

# Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

## Overview

After you request the user’s permission to access their Apple Music library (see Requesting Access to Apple Music Library), you confirm that authorization and then identify Apple Music capabilities on the user’s device.

### Confirm Whether the User Authorized Access to Apple Music Library

Use SKCloudServiceController’s authorizationStatus() to check whether the user has authorized access to Apple Music Library. If the authorization status is SKCloudServiceAuthorizationStatus.notDetermined, call SKCloudServiceController’s requestAuthorization(_:) to prompt the user for access.

- Swift
- Objective-C

```
guard SKCloudServiceController.authorizationStatus() == .notDetermined else { return }
```

```
 SKCloudServiceAuthorizationStatus status = ([SKCloudServiceController authorizationStatus] == SKCloudServiceAuthorizationStatusNotDetermined);
```

If the authorization status is SKCloudServiceAuthorizationStatus.authorized, your app can proceed to determine which Apple Music capabilities (musicCatalogPlayback, musicCatalogSubscriptionEligible, or addToCloudMusicLibrary) are available on the user’s device.

- Swift
- Objective-C

```
guard SKCloudServiceController.authorizationStatus() == .authorized else { return }
fetchCurrentAppleMusicCapabilities()
```

```
if ([SKCloudServiceController authorizationStatus] == SKCloudServiceAuthorizationStatusAuthorized) {
   [self fetchCurrentAppleMusicCapabilities];
}
```

### Create a Cloud Service Controller and Its Handler to Fetch Capabilities

First, create an SKCloudServiceController object:

- Swift
- Objective-C

```
let controller = SKCloudServiceController()
```

```
SKCloudServiceController *controller = [[SKCloudServiceController alloc] init];
```

Then call its requestCapabilities(completionHandler:) method to fetch the current Apple Music capabilities, as described in the sections that follow.

### Check for the Capability to Play Apple Music Content

If you want your app to play Apple Music content, check whether `capabilities` includes musicCatalogPlayback:

- Swift
- Objective-C

```
controller.requestCapabilities {(capabilities: SKCloudServiceCapability, error: Error?) in
   guard error == nil else { return }
   if capabilities.contains(.musicCatalogPlayback) {
      // Allows playback of songs in the Apple Music catalog.
   }
}
```

```
[controller requestCapabilitiesWithCompletionHandler:^(SKCloudServiceCapability capabilities, NSError *error){
    if (error != nil) {
        // Handle error.
    } else if (capabilities & SKCloudServiceCapabilityMusicCatalogPlayback) {
         // Allows playback of songs in the Apple Music catalog.
    }
}];

```

### Check for the Subscription-Eligible Capability

A user is eligible for an Apple Music subscription offer when `capabilities` doesn’t include musicCatalogPlayback but contains musicCatalogSubscriptionEligible. If you want your app to present the user with an offer to subscribe to Apple Music, check `capabilities` for these features:

- Swift
- Objective-C

```
controller.requestCapabilities {(capabilities: SKCloudServiceCapability, error: Error?) in
   guard error == nil else { return } 
   if capabilities.contains(.musicCatalogSubscriptionEligible) && !capabilities.contains(.musicCatalogPlayback) {
      // Allows subscription to the Apple Music catalog.
   }
}
```

```
[controller requestCapabilitiesWithCompletionHandler:^(SKCloudServiceCapability capabilities, NSError *error){
    if (error != nil) {
        // Handle error.
    } else if ((capabilities & SKCloudServiceCapabilityMusicCatalogSubscriptionEligible) && (!(capabilities & SKCloudServiceCapabilityMusicCatalogPlayback))) {
         // Allows subscription to the Apple Music catalog.
    }
}];
```

You can present the offer using SKCloudServiceSetupViewController.

### Check for the Capability to Add Songs to the User’s iCloud Music Library

If you want your app to add tracks to the user’s iCloud music library, check whether `capabilities` includes addToCloudMusicLibrary:

- Swift
- Objective-C

```
controller.requestCapabilities {(capabilities: SKCloudServiceCapability, error: Error?) in
   guard error == nil else { return }
   if capabilities.contains(.addToCloudMusicLibrary) {
       // Allows songs to be added to the user’s iCloud music library.
    }
}
```

```
[controller requestCapabilitiesWithCompletionHandler:^(SKCloudServiceCapability capabilities, NSError *error){
    if (error != nil) {
        // Handle error.
    } else if (capabilities & SKCloudServiceCapabilityAddToCloudMusicLibrary) {
         // Allows songs to be added to the user’s iCloud music library.
    }
}];
```

## See Also

### Determining capabilities

func requestUserToken(forDeveloperToken: String, completionHandler: (String?, (any Error)?) -> Void)

Returns a user token that you use to access personalized Apple Music content.

Deprecated

func requestStorefrontCountryCode(completionHandler: (String?, (any Error)?) -> Void)

Gets the country code for the storefront associated with a customer’s iTunes account.

Deprecated

func requestCapabilities(completionHandler: (SKCloudServiceCapability, (any Error)?) -> Void)

Gets the current capabilities associated with the Music library on the device.

Deprecated

struct SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

Deprecated

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

Deprecated

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

