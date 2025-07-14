

- SwiftUI
- EnvironmentValues
-  isFocusEffectEnabled 

Instance Property

# isFocusEffectEnabled

A Boolean value that indicates whether the view associated with this environment allows focus effects to be displayed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var isFocusEffectEnabled: Bool { get set }
```

## Discussion

The default value is `true`.

## See Also

### Configuring effects

func focusEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display focus effects, such as a default focus ring or hover effect.

