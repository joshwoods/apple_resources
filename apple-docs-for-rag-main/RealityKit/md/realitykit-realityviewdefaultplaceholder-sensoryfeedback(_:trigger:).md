

- RealityKit
- RealityViewDefaultPlaceholder
-  sensoryFeedback(\_:trigger:) 

Instance Method

# sensoryFeedback(\_:trigger:)

Plays the specified `feedback` when the provided `trigger` value changes.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func sensoryFeedback(
    _ feedback: SensoryFeedback,
    trigger: T
) -> some View where T : Equatable
```

## Parameters 

`feedback`  

Which type of feedback to play.

`trigger`  

A value to monitor for changes to determine when to play.

## Discussion

For example, you could play feedback when a state value changes:

```
struct MyView: View {
    @State private var showAccessory = false

    var body: some View {
        ContentView()
            .sensoryFeedback(.selection, trigger: showAccessory)
            .onLongPressGesture {
                showAccessory.toggle()
            }

        if showAccessory {
            AccessoryView()
        }
    }
}
```

