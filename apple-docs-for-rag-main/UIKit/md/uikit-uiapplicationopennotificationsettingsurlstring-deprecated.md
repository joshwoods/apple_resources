

- UIKit
-  UIApplicationOpenNotificationSettingsURLString Deprecated

Global Variable

# UIApplicationOpenNotificationSettingsURLString

A constant that provides the URL string you use to deep link to your app’s notification settings in the Settings app.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 15.4–16.0DeprecatedtvOS 15.4–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
nonisolated
let UIApplicationOpenNotificationSettingsURLString: String
```

Deprecated

In Swift, use openNotificationSettingsURLString instead.

## Discussion

Create a URL from this value and pass it to the open(_:options:completionHandler:) method to launch the Settings app and display your app’s notification settings, if it has any.

```
// Create the URL that deep links to your app's notification settings.
NSURL *url = [[NSURL alloc] initWithString:UIApplicationOpenNotificationSettingsURLString];
// Ask the system to open that URL.
[[UIApplication sharedApplication] openURL:url
                                   options:@{}
                         completionHandler:nil];
```

## See Also

### Deep linking to custom settings

class let openSettingsURLString: String

The URL string you use to deep link to your app’s custom settings in the Settings app.

static let openNotificationSettingsURLString: String

The URL string you use to deep link to your app’s notification settings in the Settings app.

class let openDefaultApplicationsSettingsURLString: String

The URL string used to select a default app in the Settings app.

