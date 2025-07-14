

- SwiftUI
-  Accessible appearance 

API Collection

# Accessible appearance

Enhance the legibility of content in your app’s interface.

## Overview

Make content easier for people to see by making it larger, giving it greater contrast, or reducing the amount of distracting motion.

For design guidance, see Accessibility in the Accessibility section of the Human Interface Guidelines.

## Topics

### Managing color

func accessibilityIgnoresInvertColors(Bool) -> some View

Sets whether this view should ignore the system Smart Invert setting.

var accessibilityInvertColors: Bool

Whether the system preference for Invert Colors is enabled.

var accessibilityDifferentiateWithoutColor: Bool

Whether the system preference for Differentiate without Color is enabled.

### Enlarging content

func accessibilityShowsLargeContentViewer() -> some View

Adds a default large content view to be shown by the large content viewer.

func accessibilityShowsLargeContentViewer&lt;V>(() -> V) -> some View

Adds a custom large content view to be shown by the large content viewer.

var accessibilityLargeContentViewerEnabled: Bool

Whether the Large Content Viewer is enabled.

### Improving legibility

var accessibilityShowButtonShapes: Bool

Whether the system preference for Show Button Shapes is enabled.

var accessibilityReduceTransparency: Bool

Whether the system preference for Reduce Transparency is enabled.

var legibilityWeight: LegibilityWeight?

The font weight to apply to text.

enum LegibilityWeight

The Accessibility Bold Text user setting options.

### Minimizing motion

var accessibilityDimFlashingLights: Bool

Whether the setting to reduce flashing or strobing lights in video content is on. This setting can also be used to determine if UI in playback controls should be shown to indicate upcoming content that includes flashing or strobing lights.

var accessibilityPlayAnimatedImages: Bool

Whether the setting for playing animations in an animated image is on. When this value is false, any presented image that contains animation should not play automatically.

var accessibilityReduceMotion: Bool

Whether the system preference for Reduce Motion is enabled.

### Using assistive access

var accessibilityAssistiveAccessEnabled: Bool

A Boolean value that indicates whether Assistive Access is in use.

## See Also

### Accessibility

Accessibility fundamentals

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Accessible controls

Improve access to actions that your app can undertake.

Accessible descriptions

Describe interface elements to help people understand what they represent.

Accessible navigation

Enable users to navigate to specific user interface elements using rotors.

