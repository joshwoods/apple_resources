

- SwiftUI
-  ColorSchemeContrast 

Enumeration

# ColorSchemeContrast

The contrast between the app’s foreground and background colors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum ColorSchemeContrast
```

## Overview

You receive a contrast value when you read the colorSchemeContrast environment value. The value tells you if a standard or increased contrast currently applies to the view. SwiftUI updates the value whenever the contrast changes, and redraws views that depend on the value. For example, the following Text view automatically updates when the user enables increased contrast:

```
@Environment(\.colorSchemeContrast) private var colorSchemeContrast

var body: some View {
    Text(colorSchemeContrast == .standard ? "Standard" : "Increased")
}
```

The user sets the contrast by selecting the Increase Contrast option in Accessibility \> Display in System Preferences on macOS, or Accessibility \> Display & Text Size in the Settings app on iOS. Your app can’t override the user’s choice. For information about using color and contrast in your app, see Accessibility in the Human Interface Guidelines.

## Topics

### Getting contrast options

case standard

SwiftUI displays views with standard contrast between the app’s foreground and background colors.

case increased

SwiftUI displays views with increased contrast between the app’s foreground and background colors.

### Creating a color scheme contrast

init?(UIAccessibilityContrast)

Creates a contrast from its accessibility contrast equivalent.

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the color scheme contrast

var colorSchemeContrast: ColorSchemeContrast

The contrast associated with the color scheme of this environment.

