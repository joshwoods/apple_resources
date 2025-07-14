

- UIKit
- UIApplication
-  openSettingsURLString 

Type Property

# openSettingsURLString

The URL string you use to deep link to your app’s custom settings in the Settings app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let openSettingsURLString: String
```

## Discussion

Create a URL from this value and pass it to the open(_:options:completionHandler:) method to launch the Settings app and display your app’s custom settings, if it has any.

- Swift
- Objective-C

```
// Create the URL that deep links to your app's custom settings.
if let url = URL(string: UIApplication.openSettingsURLString) {
    // Ask the system to open that URL.
    await UIApplication.shared.open(url)
}
```

```
// Create the URL that deep links to your app's custom settings.
NSURL *url = [[NSURL alloc] initWithString:UIApplicationOpenSettingsURLString];
// Ask the system to open that URL.
[[UIApplication sharedApplication] openURL:url
                                   options:@{}
                         completionHandler:nil];
```

For design guidance, see Human Interface Guidelines.

## See Also

### Deep linking to custom settings

static let openNotificationSettingsURLString: String

The URL string you use to deep link to your app’s notification settings in the Settings app.

let UIApplicationOpenNotificationSettingsURLString: String

A constant that provides the URL string you use to deep link to your app’s notification settings in the Settings app.

Deprecated

class let openDefaultApplicationsSettingsURLString: String

The URL string used to select a default app in the Settings app.

