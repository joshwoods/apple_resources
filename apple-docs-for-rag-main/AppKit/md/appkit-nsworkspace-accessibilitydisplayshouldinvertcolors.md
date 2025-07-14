

- AppKit
- NSWorkspace
-  accessibilityDisplayShouldInvertColors 

Instance Property

# accessibilityDisplayShouldInvertColors

A Boolean value that indicates whether the accessibility option to invert colors is in an enabled state.

macOS 10.12+

``` source
var accessibilityDisplayShouldInvertColors: Bool { get }
```

## Discussion

If this property’s value is true, the system inverts the display. In this case, you may need to adjust your app’s drawing for optimal display. To receive updates when this setting changes, register for the accessibilityDisplayOptionsDidChangeNotification notification using notificationCenter.

## See Also

### Supporting Accessibility

var accessibilityDisplayShouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the app avoids conveying information through color alone.

var accessibilityDisplayShouldIncreaseContrast: Bool

A Boolean value that indicates whether the app presents a high-contrast user interface.

var accessibilityDisplayShouldReduceTransparency: Bool

A Boolean value that indicates whether the app avoids using semitransparent backgrounds.

var accessibilityDisplayShouldReduceMotion: Bool

A Boolean value that indicates whether the accessibility option to reduce motion is in an enabled state.

var isSwitchControlEnabled: Bool

A Boolean value that indicates whether Switch Control is currently running.

var isVoiceOverEnabled: Bool

A Boolean value that indicates whether VoiceOver is currently running.

