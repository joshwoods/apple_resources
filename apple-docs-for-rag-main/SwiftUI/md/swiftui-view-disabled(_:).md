

- SwiftUI
- View
-  disabled(\_:) 

Instance Method

# disabled(\_:)

Adds a condition that controls whether users can interact with this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func disabled(_ disabled: Bool) -> some View
```

## Parameters 

`disabled`  

A Boolean value that determines whether users can interact with this view.

## Return Value

A view that controls whether users can interact with this view.

## Discussion

The higher views in a view hierarchy can override the value you set on this view. In the following example, the button isn’t interactive because the outer `disabled(_:)` modifier overrides the inner one:

```
HStack {
    Button(Text("Press")) {}
    .disabled(false)
}
.disabled(true)
```

## See Also

### Managing view interaction

var isEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows user interaction.

func interactionActivityTrackingTag(String) -> some View

Sets a tag that you use for tracking interactivity.

func invalidatableContent(Bool) -> some View

Mark the receiver as their content might be invalidated.

