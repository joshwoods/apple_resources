

- AppKit
- NSWorkspace
-  accessibilityDisplayShouldReduceTransparency 

Instance Property

# accessibilityDisplayShouldReduceTransparency

A Boolean value that indicates whether the app avoids using semitransparent backgrounds.

macOS 10.10+

``` source
var accessibilityDisplayShouldReduceTransparency: Bool { get }
```

## Discussion

If this property is true, don’t use semitransparent backgrounds in the user interface. For example, use only opaque windows.

Users can change this setting by choosing System Preferences \> Accessibility \> Display and selecting the “Reduce transparency” option. To receive updates when this setting changes, register to the accessibilityDisplayOptionsDidChangeNotification notification using notificationCenter.

## See Also

### Supporting Accessibility

var accessibilityDisplayShouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the app avoids conveying information through color alone.

var accessibilityDisplayShouldIncreaseContrast: Bool

A Boolean value that indicates whether the app presents a high-contrast user interface.

var accessibilityDisplayShouldInvertColors: Bool

A Boolean value that indicates whether the accessibility option to invert colors is in an enabled state.

var accessibilityDisplayShouldReduceMotion: Bool

A Boolean value that indicates whether the accessibility option to reduce motion is in an enabled state.

var isSwitchControlEnabled: Bool

A Boolean value that indicates whether Switch Control is currently running.

var isVoiceOverEnabled: Bool

A Boolean value that indicates whether VoiceOver is currently running.

