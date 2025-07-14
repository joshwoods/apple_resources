

- App Intents
- SiriTipView
-  scrollClipDisabled(\_:) 

Instance Method

# scrollClipDisabled(\_:)

Sets whether a scroll view clips its content to its bounds.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func scrollClipDisabled(_ disabled: Bool = true) -> some View
```

## Parameters 

`disabled`  

A Boolean value that specifies whether to disable scroll view clipping.

## Return Value

A view that disables or enables scroll view clipping.

## Discussion

By default, a scroll view clips its content to its bounds, but you can disable that behavior by using this modifier. For example, if the views inside the scroll view have shadows that extend beyond the bounds of the scroll view, you can use this modifier to avoid clipping the shadows:

```
struct ContentView: View {
    var disabled: Bool
    let colors: [Color] = [.red, .green, .blue, .mint, .teal]

    var body: some View {
        ScrollView(.horizontal) {
            HStack(spacing: 20) {
                ForEach(colors, id: \.self) { color in
                    Rectangle()
                        .frame(width: 100, height: 100)
                        .foregroundStyle(color)
                        .shadow(color: .primary, radius: 20)
                }
            }
        }
        .scrollClipDisabled(disabled)
    }
}
```

The scroll view in the above example clips when the content view’s `disabled` input is `false`, as it does if you omit the modifier, but not when the input is `true`:

- True
- False

While you might want to avoid clipping parts of views that exceed the bounds of the scroll view, like the shadows in the above example, you typically still want the scroll view to clip at some point. Create custom clipping by using the `View/clipShape(_:style:)` modifier to add a different clip shape. The following code disables the default clipping and then adds rectangular clipping that exceeds the bounds of the scroll view by the default padding amount:

```
ScrollView(.horizontal) {
    // ...
}
.scrollClipDisabled()
.padding()
.clipShape(Rectangle())
```

