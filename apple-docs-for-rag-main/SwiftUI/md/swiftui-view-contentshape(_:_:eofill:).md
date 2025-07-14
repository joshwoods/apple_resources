

- SwiftUI
- View
-  contentShape(\_:\_:eoFill:) 

Instance Method

# contentShape(\_:\_:eoFill:)

Sets the content shape for this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func contentShape(
    _ kind: ContentShapeKinds,
    _ shape: S,
    eoFill: Bool = false
) -> some View where S : Shape
```

## Parameters 

`kind`  

The kinds to apply to this content shape.

`shape`  

The shape to use.

`eoFill`  

A Boolean that indicates whether the shape is interpreted with the even-odd winding number rule.

## Return Value

A view that uses the given shape for the specified kind.

## Mentioned in 

Making a view into a drag source

## Discussion

The content shape has a variety of uses. You can control the kind of the content shape by specifying one in `kind`. The following example sets the focus ring shape of the view, without affecting its shape for hit-testing:

```
MyFocusableView()
    .contentShape(.focusEffect, Circle())
```

You can apply multiple kinds of content shapes to the same view. For example, apply a interaction shape and focusEffect shape together to set both the hit-testing shape and focus ring shape on a view.

## Context Menu &amp; Drag Previews

You can control the preview shown by the system for context menus or drags using the relevant content shape kind, like dragPreview and contextMenuPreview.

The following example creates a VStack of an Image and Text that has a context menu with a custom content shape:

```
VStack {
    Image("turtlerock")
        .contentShape(.contextMenuPreview,
                      RoundedRectangle(cornerRadius: 10))
    Text("Turtle Rock")
}
.contextMenu {
    Button {
        // Add this item to a list of favorites.
    } label: {
        Label("Add to Favorites", systemImage: "heart")
    }
}
```

When someone activates the context menu with an action like touch and hold in iOS or iPadOS, the system uses the Image as the preview for the context menu, applying the requested corner radius.

The content shape also supports applying modifiers such as inset(by:) to add padding.

Note

Similar to focusEffect, the contextMenuPreview and dragPreview content shapes do not impact the hit-testing shape. In this example, someone can touch and hold anywhere on the VStack to activate the menu. If you only want the Image to activate the menu, apply contextMenu(menuItems:) to the Image instead.

## See Also

### Controlling hit testing

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func contentShape&lt;S>(S, eoFill: Bool) -> some View

Defines the content shape for hit testing.

struct ContentShapeKinds

A kind for the content shape of a view.

