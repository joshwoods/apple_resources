

- FamilyControls
- FamilyActivityIconView
-  allowsTightening(\_:) 

Instance Method

# allowsTightening(\_:)

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func allowsTightening(_ flag: Bool) -> some View
```

## Parameters 

`flag`  

A Boolean value that indicates whether the space between characters compresses when necessary.

## Return Value

A view that can compress the space between characters when necessary to fit text in a line.

## Discussion

Use `allowsTightening(_:)` to enable the compression of inter-character spacing of text in a view to try to fit the text in the view’s bounds.

In the example below, two identically configured text views show the effects of `allowsTightening(_:)` on the compression of the spacing between characters:

```
VStack {
    Text("This is a wide text element")
        .font(.body)
        .frame(width: 200, height: 50, alignment: .leading)
        .lineLimit(1)
        .allowsTightening(true)

    Text("This is a wide text element")
        .font(.body)
        .frame(width: 200, height: 50, alignment: .leading)
        .lineLimit(1)
        .allowsTightening(false)
}
```

