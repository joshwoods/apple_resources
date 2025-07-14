

- RealityKit
- ObjectCapturePointCloudView
-  sensoryFeedback(\_:trigger:condition:) 

Instance Method

# sensoryFeedback(\_:trigger:condition:)

Plays the specified `feedback` when the provided `trigger` value changes and the `condition` closure returns `true`.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func sensoryFeedback(
    _ feedback: SensoryFeedback,
    trigger: T,
    condition: @escaping (T, T) -> Bool
) -> some View where T : Equatable
```

## Parameters 

`feedback`  

Which type of feedback to play.

`trigger`  

A value to monitor for changes to determine when to play.

`condition`  

A closure to determine whether to play the feedback when `trigger` changes.

## Discussion

For example, you could play feedback for certain state transitions:

```
struct MyView: View {
    @State private var phase = Phase.inactive

    var body: some View {
        ContentView(phase: $phase)
            .sensoryFeedback(.selection, trigger: phase) { old, new in
                old == .inactive || new == .expanded
            }
    }

    enum Phase {
        case inactive
        case preparing
        case active
        case expanded
    }
}
```

