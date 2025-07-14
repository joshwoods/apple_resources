

- RealityKit
- RealityViewAttachmentBuilderContent
-  backgroundStyle(\_:) 

Instance Method

# backgroundStyle(\_:)

Sets the specified style to render backgrounds within the view.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func backgroundStyle(_ style: S) -> some View where S : ShapeStyle
```

## Discussion

The following example uses this modifier to set the `EnvironmentValues/backgroundStyle` environment value to a `ShapeStyle/blue` color that includes a subtle `Color/gradient`. SwiftUI fills the `Circle` shape that acts as a background element with this style:

```
Image(systemName: "swift")
    .padding()
    .background(in: Circle())
    .backgroundStyle(.blue.gradient)
```

To restore the default background style, set the `EnvironmentValues/backgroundStyle` environment value to `nil` using the `View/environment(_:_:)` modifer:

```
.environment(\.backgroundStyle, nil)
```

