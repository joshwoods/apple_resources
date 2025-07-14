

- UIKit
- UIApplication
-  openNotificationSettingsURLString 

Type Property

# openNotificationSettingsURLString

The URL string you use to deep link to your app’s notification settings in the Settings app.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOSvisionOS

``` source
nonisolated
static let openNotificationSettingsURLString: String
```

## Discussion

Create a URL from this value and pass it to the open(_:options:completionHandler:) method to launch the Settings app and display your app’s notification settings, if it has any.

```
// Create the URL that deep links to your app's notification settings.
if let url = URL(string: UIApplication.openNotificationSettingsURLString) {
    // Ask the system to open that URL.
    await UIApplication.shared.open(url)
}
```

## See Also

### Deep linking to custom settings

class let openSettingsURLString: String

The URL string you use to deep link to your app’s custom settings in the Settings app.

let UIApplicationOpenNotificationSettingsURLString: String

A constant that provides the URL string you use to deep link to your app’s notification settings in the Settings app.

Deprecated

class let openDefaultApplicationsSettingsURLString: String

The URL string used to select a default app in the Settings app.

