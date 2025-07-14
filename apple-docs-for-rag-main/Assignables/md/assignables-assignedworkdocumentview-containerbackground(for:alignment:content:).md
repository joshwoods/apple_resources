

- Assignables
- AssignedWorkDocumentView
-  containerBackground(for:alignment:content:) 

Instance Method

# containerBackground(for:alignment:content:)

Sets the container background of the enclosing container using a view.

AssignablesSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func containerBackground(
    for container: ContainerBackgroundPlacement,
    alignment: Alignment = .center,
    @ViewBuilder content: () -> V
) -> some View where V : View
```

## Parameters 

`alignment`  

The alignment that the modifier uses to position the implicit `ZStack` that groups the background views. The default is `Alignment/center`.

`container`  

The container that will use the background.

`content`  

The view to use as the background of the container.

## Discussion

The following example uses a custom `View` as a background:

```
struct ContentView: View {
    var body: some View {
        NavigationStack {
            List {
                NavigationLink("Image") {
                    Text("Image")
                    .containerBackground(for: .navigation) {
                        Image(name: "ImageAsset")
                    }
                }
            }
        }
    }
}
```

The `.containerBackground(for:alignment:content:)` modifier differs from the `View/background(_:ignoresSafeAreaEdges:)` modifier by automatically filling an entire parent container. `ContainerBackgroundPlacement` describes the available containers.

