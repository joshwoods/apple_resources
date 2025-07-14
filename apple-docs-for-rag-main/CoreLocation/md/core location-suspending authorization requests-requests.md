

- Core Location
-  Suspending authorization requests 

Article

# Suspending authorization requests

Defer the system’s authorization request dialog until your app is ready.

## Overview

If your app has an onboarding flow that includes obtaining location updates, you may want to defer the Core Location’s request for authorization from the user. You can inhibit the auto-prompting in your app by creating a CLServiceSession at a convenient time in your app, then iterating over its diagnostics property to determine the level of authorization the person using your app selects. The following code snippet demonstrates how to defer the prompting.

```
func doPromptingFlow() async {
    await showHelloPrompt()

    // Obtain a session. This causes Core Location to display the authorization prompt.
    let session = CLServiceSession.session(authorization: .whenInUse)

    // Wait for interaction with the prompot to complete (successfully or with denial).
    for try await diagnostic in session.diagnostics {
        if !diagnostic.authorizationRequestInProgress {
            // A denial occurred.
            break
        }
    }

    await doFurtherWork()
}
```

Add the `CLRequireExplicitServiceSession` property to your app’s Info.plist file to opt into this control behavior.

## See Also

### Authorization

Requesting authorization to use location services

Obtain authorization to use location services and manage changes to your app’s authorization status.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

enum CLAccuracyAuthorization

Constants that indicate the level of location accuracy the app has authorization to use.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

Deprecated

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

Deprecated

