

- WebKit
- WKPreferences
-  isElementFullscreenEnabled 

Instance Property

# isElementFullscreenEnabled

A Boolean value that indicates whether a web view can display content full screen.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+visionOS 1.0+

``` source
@MainActor
var isElementFullscreenEnabled: Bool { get set }
```

## Discussion

The default value for this preference is false.

Important

When this value is true and a page requests full-screen mode, the system removes the WKWebView from your app’s view hierarchy.

## See Also

### Setting Behavior Preferences

var tabFocusesLinks: Bool

A Boolean value that indicates whether pressing the tab key changes the focus to links and form controls.

var isTextInteractionEnabled: Bool

A Boolean value that indicates whether to allow people to select or otherwise interact with text.

var inactiveSchedulingPolicy: WKPreferences.InactiveSchedulingPolicy

A policy you set to specify how a web view that’s not in a window handles tasks.

enum InactiveSchedulingPolicy

An enumeration that lists policies for how a web view that’s not in a window handles tasks.

