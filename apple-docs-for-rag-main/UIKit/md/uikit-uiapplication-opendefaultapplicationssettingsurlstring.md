

- UIKit
- UIApplication
-  openDefaultApplicationsSettingsURLString 

Type Property

# openDefaultApplicationsSettingsURLString

The URL string used to select a default app in the Settings app.

iOS 18.3+iPadOS 18.3+Mac Catalyst 18.3+tvOS 18.3+visionOS 2.3+

``` source
nonisolated
class let openDefaultApplicationsSettingsURLString: String
```

## Discussion

Create a URL from this value and pass it to the open(_:options:completionHandler:) method to launch the Settings app and display your app’s custom settings, if it has any:

- Swift
- Objective-C

```
// Create the URL that links to the Settings app for default app selection.
if let url = URL(string: UIApplication.openDefaultApplicationsSettingsURLString) {
    // Ask the system to open that URL.
    await UIApplication.shared.open(url)
}
```

```
// Create the URL that links to the Settings app for default app selection.
NSURL *url = [[NSURL alloc] initWithString:UIApplicationOpenDefaultApplicationsSettingsURLString];
// Ask the system to open that URL.
[[UIApplication sharedApplication] openURL:url
                                   options:@{}
                         completionHandler:nil];
```

For design guidance, see Human Interface Guidelines \> Settings.

## See Also

### Deep linking to custom settings

class let openSettingsURLString: String

The URL string you use to deep link to your app’s custom settings in the Settings app.

static let openNotificationSettingsURLString: String

The URL string you use to deep link to your app’s notification settings in the Settings app.

let UIApplicationOpenNotificationSettingsURLString: String

A constant that provides the URL string you use to deep link to your app’s notification settings in the Settings app.

Deprecated

