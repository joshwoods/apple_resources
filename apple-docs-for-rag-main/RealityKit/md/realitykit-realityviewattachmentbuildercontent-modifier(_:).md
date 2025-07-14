

- RealityKit
- RealityViewAttachmentBuilderContent
-  modifier(\_:) 

Instance Method

# modifier(\_:)

Applies a modifier to a view and returns a new view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func modifier(_ modifier: T) -> ModifiedContent
```

## Parameters 

`modifier`  

The modifier to apply to this view.

## Discussion

Use this modifier to combine a `View` and a `ViewModifier`, to create a new view. For example, if you create a view modifier for a new kind of caption with blue text surrounded by a rounded rectangle:

```
struct BorderedCaption: ViewModifier {
    func body(content: Content) -> some View {
        content
            .font(.caption2)
            .padding(10)
            .overlay(
                RoundedRectangle(cornerRadius: 15)
                    .stroke(lineWidth: 1)
            )
            .foregroundColor(Color.blue)
    }
}
```

You can use modifier(_:) to extend `View` to create new modifier for applying the `BorderedCaption` defined above:

```
extension View {
    func borderedCaption() -> some View {
        modifier(BorderedCaption())
    }
}
```

Then you can apply the bordered caption to any view:

```
Image(systemName: "bus")
    .resizable()
    .frame(width:50, height:50)
Text("Downtown Bus")
    .borderedCaption()
```

