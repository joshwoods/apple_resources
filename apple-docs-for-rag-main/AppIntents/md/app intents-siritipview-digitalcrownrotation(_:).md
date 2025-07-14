

- App Intents
- SiriTipView
-  digitalCrownRotation(\_:) 

Instance Method

# digitalCrownRotation(\_:)

Tracks Digital Crown rotations by updating the specified binding.

AppIntentsSwiftUIwatchOS 6.0+

``` source
nonisolated
func digitalCrownRotation(_ binding: Binding) -> some View where V : BinaryFloatingPoint
```

## Parameters 

`binding`  

A binding to a value that updates as the user rotates the Digital Crown. The implicit range is `(-infinity, +infinity)`.

## Discussion

Use this method to receive values on a binding you provide as the user turns the Digital Crown on Apple Watch. The example below receives changes to the binding value, starting at `0.0` and incrementing or decrementing depending on the direction that the user turns the Digital Crown:

```
struct DigitalCrown: View {
    @State private var crownValue = 0.0

    var body: some View {
        Text("Received Value:\(crownValue, specifier: "%.1f")")
            .focusable()
            .digitalCrownRotation($crownValue)
    }
}
```

