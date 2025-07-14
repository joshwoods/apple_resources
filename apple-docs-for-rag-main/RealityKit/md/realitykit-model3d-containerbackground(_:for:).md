

- RealityKit
- Model3D
-  containerBackground(\_:for:) 

Instance Method

# containerBackground(\_:for:)

Sets the container background of the enclosing container using a view.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func containerBackground(
    _ style: S,
    for container: ContainerBackgroundPlacement
) -> some View where S : ShapeStyle
```

## Discussion

The following example uses a `LinearGradient` as a background:

```
struct ContentView: View {
    var body: some View {
        NavigationStack {
            List {
                NavigationLink("Blue") {
                    Text("Blue")
                    .containerBackground(.blue.gradient, for: .navigation)
                }
                NavigationLink("Red") {
                    Text("Red")
                    .containerBackground(.red.gradient, for: .navigation)
                }
            }
        }
    }
}
```

The `.containerBackground(_:for:)` modifier differs from the `View/background(_:ignoresSafeAreaEdges:)` modifier by automatically filling an entire parent container. `ContainerBackgroundPlacement` describes the available containers.

- Parameters

  - style: The shape style to use as the container background.

  - container: The container that will use the background.

