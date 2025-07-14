

- AppKit
- NSWorkspace
-  accessibilityDisplayShouldIncreaseContrast 

Instance Property

# accessibilityDisplayShouldIncreaseContrast

A Boolean value that indicates whether the app presents a high-contrast user interface.

macOS 10.10+

``` source
var accessibilityDisplayShouldIncreaseContrast: Bool { get }
```

## Discussion

When this method returns true, present a high-contrast UI. For example, use a less subtle color palette or bolder lines.

Users can change this setting by choosing System Preferences \> Accessibility \> Display and selecting the “Increase contrast” option. To receive updates when this setting changes, register for the accessibilityDisplayOptionsDidChangeNotification notification using notificationCenter.

## See Also

### Supporting Accessibility

var accessibilityDisplayShouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the app avoids conveying information through color alone.

var accessibilityDisplayShouldReduceTransparency: Bool

A Boolean value that indicates whether the app avoids using semitransparent backgrounds.

var accessibilityDisplayShouldInvertColors: Bool

A Boolean value that indicates whether the accessibility option to invert colors is in an enabled state.

var accessibilityDisplayShouldReduceMotion: Bool

A Boolean value that indicates whether the accessibility option to reduce motion is in an enabled state.

var isSwitchControlEnabled: Bool

A Boolean value that indicates whether Switch Control is currently running.

var isVoiceOverEnabled: Bool

A Boolean value that indicates whether VoiceOver is currently running.

