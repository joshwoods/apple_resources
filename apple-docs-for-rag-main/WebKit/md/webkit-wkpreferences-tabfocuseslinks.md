

- WebKit
- WKPreferences
-  tabFocusesLinks 

Instance Property

# tabFocusesLinks

A Boolean value that indicates whether pressing the tab key changes the focus to links and form controls.

macOS 10.12.4+

``` source
@MainActor
var tabFocusesLinks: Bool { get set }
```

## Discussion

When the value of this property is true, the web view includes links and form controls in the set of items that may receive focus. Pressing the Option key temporarily reverses this preference.

## See Also

### Setting Behavior Preferences

var isTextInteractionEnabled: Bool

A Boolean value that indicates whether to allow people to select or otherwise interact with text.

var isElementFullscreenEnabled: Bool

A Boolean value that indicates whether a web view can display content full screen.

var inactiveSchedulingPolicy: WKPreferences.InactiveSchedulingPolicy

A policy you set to specify how a web view that’s not in a window handles tasks.

enum InactiveSchedulingPolicy

An enumeration that lists policies for how a web view that’s not in a window handles tasks.

