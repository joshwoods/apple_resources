

- RealityKit
- RealityView
-  toolbar(content:) 

Instance Method

# toolbar(content:)

Populates the toolbar or navigation bar with the views you provide.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func toolbar(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Parameters 

`content`  

The views representing the content of the toolbar.

## Discussion

Use this modifier to add content to the toolbar. The toolbar modifier expects a collection of toolbar items that you can provide either by supplying a collection of views with each view wrapped in a `ToolbarItem`, or by providing a collection of views as a `ToolbarItemGroup`. The example below adds views to using a toolbar item group to support text editing features:

```
struct StructToolbarItemGroupView: View {
    @State private var text = ""
    @State private var bold = false
    @State private var italic = false
    @State private var fontSize = 12.0

    var displayFont: Font {
        let font = Font.system(size: CGFloat(fontSize),
                               weight: bold == true ? .bold : .regular)
        return italic == true ? font.italic() : font
    }

    var body: some View {
        TextEditor(text: $text)
            .font(displayFont)
            .toolbar {
                ToolbarItemGroup {
                    Slider(
                        value: $fontSize,
                        in: 8...120,
                        minimumValueLabel:
                            Text("A").font(.system(size: 8)),
                        maximumValueLabel:
                            Text("A").font(.system(size: 16))
                    ) {
                        Text("Font Size (\(Int(fontSize)))")
                    }
                    .frame(width: 150)
                    Toggle(isOn: $bold) {
                        Image(systemName: "bold")
                    }
                    Toggle(isOn: $italic) {
                        Image(systemName: "italic")
                    }
                }
            }
            .navigationTitle("My Note")
    }
}
```

