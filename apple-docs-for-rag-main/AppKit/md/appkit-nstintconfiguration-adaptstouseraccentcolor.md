

- AppKit
- NSTintConfiguration
-  adaptsToUserAccentColor 

Instance Property

# adaptsToUserAccentColor

A Boolean value that indicates whether the tint configuration alters its effect based on the user’s preferred accent color choice.

macOS 11.0+

``` source
var adaptsToUserAccentColor: Bool { get }
```

## Discussion

When this property is `YES`, the tint configuration alters it effect based on the user’s preferred accent color. Otherwise, the tint configuration produces a constant effect regardless of the accent color preference.

