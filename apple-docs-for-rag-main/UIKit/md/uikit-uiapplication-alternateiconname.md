

- UIKit
- UIApplication
-  alternateIconName 

Instance Property

# alternateIconName

The name of the icon the system displays for the app.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 10.2+visionOS 1.0+

``` source
@MainActor
var alternateIconName: String? { get }
```

## Discussion

When the system is displaying one of your app’s alternate icons, the value of this property is the name of the alternate icon (from your app’s `Info.plist` file). When the system is displaying your app’s primary icon, the value of this property is `nil`.

## See Also

### Managing the app’s icon

var supportsAlternateIcons: Bool

A Boolean value that indicates whether the app is allowed to change its icon.

func setAlternateIconName(String?, completionHandler: (((any Error)?) -> Void)?)

Changes the icon the system displays for the app.

