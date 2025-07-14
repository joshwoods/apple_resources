

- App Intents
- CameraCaptureIntent
-  appContext 

Type Property

# appContext

An app context that an app can use to pass necessary information to the sandboxed capture extension. The system will retrieve this app context when necessary and inject it for use during

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
static var appContext: Self.AppContext? { get async throws }
```

