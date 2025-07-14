

- Assignables
- AssignableDocumentView
-  flipsForRightToLeftLayoutDirection(\_:) 

Instance Method

# flipsForRightToLeftLayoutDirection(\_:)

Sets whether this view mirrors its contents horizontally when the layout direction is right-to-left.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func flipsForRightToLeftLayoutDirection(_ enabled: Bool) -> some View
```

## Parameters 

`enabled`  

A Boolean value that indicates whether this view should have its content flipped horizontally when the layout direction is right-to-left. By default, views will adjust their layouts automatically in a right-to-left context and do not need to be mirrored.

## Return Value

A view that conditionally mirrors its contents horizontally when the layout direction is right-to-left.

## Discussion

Use `flipsForRightToLeftLayoutDirection(_:)` when you need the system to horizontally mirror the contents of the view when presented in a right-to-left layout.

To override the layout direction for a specific view, use the `View/environment(_:_:)` view modifier to explicitly override the `EnvironmentValues/layoutDirection` environment value for the view.

