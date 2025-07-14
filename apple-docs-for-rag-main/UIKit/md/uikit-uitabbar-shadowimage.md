

- UIKit
- UITabBar
-  shadowImage 

Instance Property

# shadowImage

The shadow image to use for the tab bar.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shadowImage: UIImage? { get set }
```

## Discussion

For tab bars with custom backgrounds, you can use this property to specify a custom shadow image for your bar. The shadow image is positioned outside the bounds of the tab bar itself, usually above or below the tab bar’s frame rectangle. The exact position depends on the current platform. For example, shadow images are positioned above the tab bar on iPhone and iPad.

You must use this property in conjunction with a custom background image. If the backgroundImage property is `nil`, the tab bar ignores the value in this property and uses a default shadow.

