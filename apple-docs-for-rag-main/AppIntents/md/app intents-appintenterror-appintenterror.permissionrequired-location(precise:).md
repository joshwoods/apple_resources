

- App Intents
- AppIntentError
- AppIntentError.PermissionRequired
-  location(precise:) 

Type Method

# location(precise:)

User needs to grant location permission to the app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func location(precise: Bool = false) -> AppIntentError
```

## Discussion

The error message will differ based on whether they need to grant Precise or Approximate Location.

