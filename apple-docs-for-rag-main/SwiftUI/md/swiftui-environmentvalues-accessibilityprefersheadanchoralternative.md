

- SwiftUI
- EnvironmentValues
-  accessibilityPrefersHeadAnchorAlternative 

Instance Property

# accessibilityPrefersHeadAnchorAlternative

Whether the system setting to prefer alternatives to head-anchored content is on.

visionOS 1.0+

``` source
var accessibilityPrefersHeadAnchorAlternative: Bool { get }
```

## Discussion

If this property’s value is true, alternate anchors should be used for most head-anchored UI, such as world anchors.

## See Also

### Accessibility

var accessibilityAssistiveAccessEnabled: Bool

A Boolean value that indicates whether Assistive Access is in use.

var accessibilityDimFlashingLights: Bool

Whether the setting to reduce flashing or strobing lights in video content is on. This setting can also be used to determine if UI in playback controls should be shown to indicate upcoming content that includes flashing or strobing lights.

var accessibilityDifferentiateWithoutColor: Bool

Whether the system preference for Differentiate without Color is enabled.

var accessibilityEnabled: Bool

A Boolean value that indicates whether the user has enabled an assistive technology.

var accessibilityInvertColors: Bool

Whether the system preference for Invert Colors is enabled.

var accessibilityLargeContentViewerEnabled: Bool

Whether the Large Content Viewer is enabled.

var accessibilityPlayAnimatedImages: Bool

Whether the setting for playing animations in an animated image is on. When this value is false, any presented image that contains animation should not play automatically.

var accessibilityQuickActionsEnabled: Bool

A Boolean that indicates whether the quick actions feature is enabled.

var accessibilityReduceMotion: Bool

Whether the system preference for Reduce Motion is enabled.

var accessibilityReduceTransparency: Bool

Whether the system preference for Reduce Transparency is enabled.

var accessibilityShowButtonShapes: Bool

Whether the system preference for Show Button Shapes is enabled.

var accessibilitySwitchControlEnabled: Bool

A Boolean value that indicates whether the Switch Control motor accessibility feature is in use.

var accessibilityVoiceOverEnabled: Bool

A Boolean value that indicates whether the VoiceOver screen reader is in use.

var legibilityWeight: LegibilityWeight?

The font weight to apply to text.

