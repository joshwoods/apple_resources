

- RealityKit
- ResolvedModel3D
-  accessibilityActions(\_:) 

Instance Method

# accessibilityActions(\_:)

Adds multiple accessibility actions to the view.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func accessibilityActions(@ViewBuilder _ content: () -> Content) -> some View where Content : View
```

## Discussion

Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. For example, this is how a dynamic number of custom action could be added to a view.

```
var isDraft: Bool

var body: some View {
    ContentView()
        .accessibilityActions {
            ForEach(actions) { action in
                Button {
                    action()
                } label: {
                    Text(action.title)
                }
            }

            if isDraft {
                Button {
                    // Handle Delete
                } label: {
                    Text("Delete")
                }
            }
        }
```

