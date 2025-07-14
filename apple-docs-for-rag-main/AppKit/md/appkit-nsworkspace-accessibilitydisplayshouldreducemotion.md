

- AppKit
- NSWorkspace
-  accessibilityDisplayShouldReduceMotion 

Instance Property

# accessibilityDisplayShouldReduceMotion

A Boolean value that indicates whether the accessibility option to reduce motion is in an enabled state.

macOS 10.12+

``` source
var accessibilityDisplayShouldReduceMotion: Bool { get }
```

## Discussion

If this property’s value is true, avoid large animations, especially those that simulate the third dimension. To receive updates when this setting changes, register for the accessibilityDisplayOptionsDidChangeNotification notification using notificationCenter.

## See Also

### Supporting Accessibility

var accessibilityDisplayShouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the app avoids conveying information through color alone.

var accessibilityDisplayShouldIncreaseContrast: Bool

A Boolean value that indicates whether the app presents a high-contrast user interface.

var accessibilityDisplayShouldReduceTransparency: Bool

A Boolean value that indicates whether the app avoids using semitransparent backgrounds.

var accessibilityDisplayShouldInvertColors: Bool

A Boolean value that indicates whether the accessibility option to invert colors is in an enabled state.

var isSwitchControlEnabled: Bool

A Boolean value that indicates whether Switch Control is currently running.

var isVoiceOverEnabled: Bool

A Boolean value that indicates whether VoiceOver is currently running.

