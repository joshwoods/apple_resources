

- StoreKit
- SKCloudServiceSetupViewController
-  Offering Apple Music Subscription in Your App 

Article

# Offering Apple Music Subscription in Your App

Allow eligible customers to subscribe to Apple Music.

## Overview

With an Apple Music membership, customers can play songs from the entire Apple Music catalog or access their iCloud music library across all their devices. You can offer users the option to sign up for an Apple Music subscription directly from your app by following these steps:

1.  Request Apple Music Library access from the customer.

2.  Determine if the customer is eligible for an Apple Music subscription.

3.  Present the sign-up subscription offer if the customer is eligible.

### Request Apple Music Library Access

The user must grant permission before your app can access Apple Music library. See Requesting Access to Apple Music Library for details. Use authorizationStatus() to determine your app’s authorization status. If the authorization status is SKCloudServiceAuthorizationStatus.authorized, your app can check if the user is eligible for an Apple Music subscription offer.

- Swift
- Objective-C

```
SKCloudServiceController.authorizationStatus() == .authorized
```

```
SKCloudServiceAuthorizationStatus status = ([SKCloudServiceController authorizationStatus] == SKCloudServiceAuthorizationStatusAuthorized); 
```

Important

When the Music app is absent on the user’s device, load(options:completionHandler:) fails to load.

### Determine if the User is Eligible for an Apple Music Subscription

After getting Apple Music access from the user, call requestCapabilities(completionHandler:) on an instance of SKCloudServiceController to query the user’s capabilities. Then, inspect the `capabilities` parameter of this method to determine eligibility. See Determining a person’s Apple Music capabilities for details. A user has an active subscription to Apple Music when `capabilities` contains musicCatalogPlayback. A user is eligible for the offer when `capabilities` doesn’t include musicCatalogPlayback but contains musicCatalogSubscriptionEligible.

- Swift
- Objective-C

```
let controller = SKCloudServiceController()
controller.requestCapabilities { (capabilities: SKCloudServiceCapability, error: Error?) in
    guard error == nil else { return }

    if capabilities.contains(.musicCatalogSubscriptionEligible) && !capabilities.contains(.musicCatalogPlayback) {
        // Allows subscription to the Apple Music catalog.
    }
}
```

```
SKCloudServiceController *controller = [[SKCloudServiceController alloc] init];

[controller requestCapabilitiesWithCompletionHandler:^(SKCloudServiceCapability capabilities, NSError *error){
     if (error != nil) {
         // Handle error.
     } else if ((capabilities & SKCloudServiceCapabilityMusicCatalogSubscriptionEligible) && (!(capabilities & SKCloudServiceCapabilityMusicCatalogPlayback))) {
         // Allows subscription to the Apple Music catalog.
     }
}];
```

### Present the Offer to Subscribe for Apple Music

For users who are eligible for an Apple Music subscription, use the following steps to allow users to sign up for it.

First, create a dictionary with an action key to subscribe:

- Swift
- Objective-C

```
let options: [SKCloudServiceSetupOptionsKey: Any] = [.action: SKCloudServiceSetupAction.subscribe]
```

```
NSDictionary *options = @{SKCloudServiceSetupOptionsActionKey: SKCloudServiceSetupActionSubscribe};
```

If you have an iTunes Store affiliate account, you can add the affiliateToken key to the dictionary to earn commision if the user subscribes:

- Swift
- Objective-C

```
let affiliateToken = "Your_Affiliate_Token"
let options: [SKCloudServiceSetupOptionsKey: Any] = [.action: SKCloudServiceSetupAction.subscribe, .affiliateToken: affiliateToken]
```

```
NSString *affiliateToken = @"Your_Affiliate_Token";
NSDictionary *options = @{SKCloudServiceSetupOptionsActionKey: SKCloudServiceSetupActionSubscribe, SKCloudServiceSetupOptionsAffiliateTokenKey: affiliateToken};
```

By default, the setup view is configured with the messageIdentifier key set to join. Add messageIdentifier to the dictionary and set it to addMusic, connect, or playMusic if you wish to change the default message that your app shows to the user:

- Swift
- Objective-C

```
let options: [SKCloudServiceSetupOptionsKey: Any] = [.action: SKCloudServiceSetupAction.subscribe, .messageIdentifier: SKCloudServiceSetupMessageIdentifier.addMusic]
```

```
NSDictionary *options = @{SKCloudServiceSetupOptionsActionKey: SKCloudServiceSetupActionSubscribe, SKCloudServiceSetupOptionsMessageIdentifierKey: SKCloudServiceSetupMessageIdentifierAddMusic};
```

Next, create an SKCloudServiceSetupViewController object and set the view controller class as its delegate:

- Swift
- Objective-C

```
let controller = SKCloudServiceSetupViewController()
controller.delegate = self
```

```
SKCloudServiceSetupViewController *controller = [[SKCloudServiceSetupViewController alloc] init];
controller.delegate = self;
```

Then, pass the dictionary to the load(options:completionHandler:) method of the SKCloudServiceSetupViewController object. Finally, present the SKCloudServiceSetupViewController object modally from your app:

- Swift
- Objective-C

```
controller.load(options: options) { [weak self] (result: Bool, error: Error?) in
   guard error == nil else { return }

    if result {
        self?.present(controller, animated: true, completion: nil)
    }
}
```

```
[controller loadWithOptions:options completionHandler:^(BOOL result, NSError *error) {
    if(error != nil) {
        // Handle error.
     } else if (result) {
        [self presentViewController:controller animated:YES completion:nil];
     }
}];
```

## See Also

### Loading the setup view

struct SKCloudServiceSetupOptionsKey

Keys to specify the types of setup options for a cloud service.

func load(options: [SKCloudServiceSetupOptionsKey : Any], completionHandler: ((Bool, (any Error)?) -> Void)?)

Loads the cloud service setup view with the specified options.

Deprecated

class SKArcadeService

