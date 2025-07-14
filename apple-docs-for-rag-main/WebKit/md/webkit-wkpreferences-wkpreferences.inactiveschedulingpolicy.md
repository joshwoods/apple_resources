

- WebKit
- WKPreferences
-  WKPreferences.InactiveSchedulingPolicy 

Enumeration

# WKPreferences.InactiveSchedulingPolicy

An enumeration that lists policies for how a web view that’s not in a window handles tasks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
enum InactiveSchedulingPolicy
```

## Topics

### Scheduling policies

case none

A policy where a web view that’s not in a window runs tasks normally.

case suspend

A policy where a web view that’s not in a window fully suspends tasks.

case throttle

A policy where a web view that’s not in a window limits processing, but does not fully suspend tasks.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting Behavior Preferences

var tabFocusesLinks: Bool

A Boolean value that indicates whether pressing the tab key changes the focus to links and form controls.

var isTextInteractionEnabled: Bool

A Boolean value that indicates whether to allow people to select or otherwise interact with text.

var isElementFullscreenEnabled: Bool

A Boolean value that indicates whether a web view can display content full screen.

var inactiveSchedulingPolicy: WKPreferences.InactiveSchedulingPolicy

A policy you set to specify how a web view that’s not in a window handles tasks.

