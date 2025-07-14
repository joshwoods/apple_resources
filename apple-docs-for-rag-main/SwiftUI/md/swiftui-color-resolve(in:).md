

- SwiftUI
- Color
-  resolve(in:) 

Instance Method

# resolve(in:)

Evaluates this color to a resolved color given the current `context`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func resolve(in environment: EnvironmentValues) -> Color.Resolved
```

## See Also

### Creating a color

init(String, bundle: Bundle?)

Creates a color from a color set that you indicate by name.

init(_:)

Creates a constant color with the values specified by the resolved color.

