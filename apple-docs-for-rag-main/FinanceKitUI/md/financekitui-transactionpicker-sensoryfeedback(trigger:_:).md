

- FinanceKitUI
- TransactionPicker
-  sensoryFeedback(trigger:\_:) 

Instance Method

# sensoryFeedback(trigger:\_:)

Plays feedback when returned from the `feedback` closure after the provided `trigger` value changes.

FinanceKitUISwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func sensoryFeedback(
    trigger: T,
    _ feedback: @escaping (T, T) -> SensoryFeedback?
) -> some View where T : Equatable
```

## Parameters 

`trigger`  

A value to monitor for changes to determine when to play.

`feedback`  

A closure to determine whether to play the feedback and what type of feedback to play when `trigger` changes.

## Discussion

For example, you could play different feedback for different state transitions:

```
struct MyView: View {
    @State private var phase = Phase.inactive

    var body: some View {
        ContentView(phase: $phase)
            .sensoryFeedback(trigger: phase) { old, new in
                switch (old, new) {
                    case (.inactive, _): return .success
                    case (_, .expanded): return .impact
                    default: return nil
                }
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

