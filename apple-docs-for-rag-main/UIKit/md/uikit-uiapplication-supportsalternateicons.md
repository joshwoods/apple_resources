

- UIKit
- UIApplication
-  supportsAlternateIcons 

Instance Property

# supportsAlternateIcons

A Boolean value that indicates whether the app is allowed to change its icon.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 10.2+visionOS 1.0+

``` source
@MainActor
var supportsAlternateIcons: Bool { get }
```

## Discussion

The value of this property is true only when the system allows you to change the icon of your app. To declare your app’s alternate icons, include them in the CFBundleIcons key of your app’s `Info.plist` file.

The value of this property is always false for apps built using the visionOS SDK.

## See Also

### Managing the app’s icon

var alternateIconName: String?

The name of the icon the system displays for the app.

func setAlternateIconName(String?, completionHandler: (((any Error)?) -> Void)?)

Changes the icon the system displays for the app.

