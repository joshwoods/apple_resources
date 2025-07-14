

- UIKit
- UISplitViewController
-  primaryBackgroundStyle 

Instance Property

# primaryBackgroundStyle

The background style of the primary view controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var primaryBackgroundStyle: UISplitViewController.BackgroundStyle { get set }
```

## Mentioned in 

Optimizing your iPad app for Mac

## Discussion

In macOS, the sidebar of a split view shows a blurred desktop behind its view. To achieve this effect in your iPad app when it runs in macOS, set primaryBackgroundStyle to UISplitViewController.BackgroundStyle.sidebar. Set the style to UISplitViewController.BackgroundStyle.none when you want to control the background appearance of the primary view controller.

Note

Setting the background style to UISplitViewController.BackgroundStyle.sidebar has no effect when your app is running in iOS or tvOS.

## See Also

### Managing the background style

enum BackgroundStyle

Styles that apply a visual effect to the background of a primary view controller.

