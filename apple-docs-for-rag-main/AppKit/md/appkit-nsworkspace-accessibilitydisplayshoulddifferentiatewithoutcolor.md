

- AppKit
- NSWorkspace
-  accessibilityDisplayShouldDifferentiateWithoutColor 

Instance Property

# accessibilityDisplayShouldDifferentiateWithoutColor

A Boolean value that indicates whether the app avoids conveying information through color alone.

macOS 10.10+

``` source
var accessibilityDisplayShouldDifferentiateWithoutColor: Bool { get }
```

## Discussion

If this property is true, the user interface avoids conveying information using color alone. Instead, use shapes or glyphs to convey important information.

Users can change this setting by choosing System Preferences \> Accessibility \> Display and selecting the “Differentiate without color” option. To receive updates when this setting changes, register for the accessibilityDisplayOptionsDidChangeNotification notification using notificationCenter.

## See Also

### Supporting Accessibility

var accessibilityDisplayShouldIncreaseContrast: Bool

A Boolean value that indicates whether the app presents a high-contrast user interface.

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

