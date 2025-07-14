

- WebKit
- WKPreferences
-  isTextInteractionEnabled 

Instance Property

# isTextInteractionEnabled

A Boolean value that indicates whether to allow people to select or otherwise interact with text.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
var isTextInteractionEnabled: Bool { get set }
```

## Discussion

The default value for this preference is true on macOS and iOS. On watchOS, the default value is false.

## See Also

### Setting Behavior Preferences

var tabFocusesLinks: Bool

A Boolean value that indicates whether pressing the tab key changes the focus to links and form controls.

var isElementFullscreenEnabled: Bool

A Boolean value that indicates whether a web view can display content full screen.

var inactiveSchedulingPolicy: WKPreferences.InactiveSchedulingPolicy

A policy you set to specify how a web view that’s not in a window handles tasks.

enum InactiveSchedulingPolicy

An enumeration that lists policies for how a web view that’s not in a window handles tasks.

