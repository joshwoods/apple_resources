

- UIKit
- UIApplicationDelegate
-  applicationShouldRequestHealthAuthorization(\_:) 

Instance Method

# applicationShouldRequestHealthAuthorization(\_:)

Tells the delegate when your app should ask the user for access to his or her HealthKit data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func applicationShouldRequestHealthAuthorization(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Discussion

In your implementation of this method, call the handleAuthorizationForExtension(completion:) method of the HKHealthStore object.

