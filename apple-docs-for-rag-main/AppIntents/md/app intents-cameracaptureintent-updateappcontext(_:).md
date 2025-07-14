

- App Intents
- CameraCaptureIntent
-  updateAppContext(\_:) 

Type Method

# updateAppContext(\_:)

Whenever the in-app context for this intent changes any process containing this intent can call this method to provide updated state to the system.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
static func updateAppContext(_ newContext: Self.AppContext?) async throws
```

## Discussion

Note: The size of data `newContext` uses when encoded with JSONEncoder can not exceed 4kB

