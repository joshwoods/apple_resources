

- SwiftUI
- EnvironmentValues
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the view associated with this environment allows user interaction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

The default value is `true`.

## See Also

### Managing view interaction

func disabled(Bool) -> some View

Adds a condition that controls whether users can interact with this view.

func interactionActivityTrackingTag(String) -> some View

Sets a tag that you use for tracking interactivity.

func invalidatableContent(Bool) -> some View

Mark the receiver as their content might be invalidated.

