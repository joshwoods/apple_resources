

- SwiftUI
-  ColorScheme 

Enumeration

# ColorScheme

The possible color schemes, corresponding to the light and dark appearances.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum ColorScheme
```

## Overview

You receive a color scheme value when you read the colorScheme environment value. The value tells you if a light or dark appearance currently applies to the view. SwiftUI updates the value whenever the appearance changes, and redraws views that depend on the value. For example, the following Text view automatically updates when the user enables Dark Mode:

```
@Environment(\.colorScheme) private var colorScheme

var body: some View {
    Text(colorScheme == .dark ? "Dark" : "Light")
}
```

Set a preferred appearance for a particular view hierarchy to override the user’s Dark Mode setting using the preferredColorScheme(_:) view modifier.

## Topics

### Getting color schemes

case light

The color scheme that corresponds to a light appearance.

case dark

The color scheme that corresponds to a dark appearance.

### Creating a color scheme

init?(UIUserInterfaceStyle)

Creates a color scheme from its user interface style equivalent.

### Supporting types

struct PreferredColorSchemeKey

A key for specifying the preferred color scheme.

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Detecting and requesting the light or dark appearance

func preferredColorScheme(ColorScheme?) -> some View

Sets the preferred color scheme for this presentation.

var colorScheme: ColorScheme

The color scheme of this environment.

