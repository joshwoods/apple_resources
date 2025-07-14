

- SwiftUI
- State
-  projectedValue 

Instance Property

# projectedValue

A binding to the state value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var projectedValue: Binding { get }
```

## Mentioned in 

Managing user interface state

## Discussion

Use the projected value to get a Binding to the stored value. The binding provides a two-way connection to the stored value. To access the `projectedValue`, prefix the property variable with a dollar sign (`$`).

In the following example, `PlayerView` projects a binding of the state property `isPlaying` to the `PlayButton` view using `$isPlaying`. That enables the play button to both read and write the value:

```
struct PlayerView: View {
    var episode: Episode
    @State private var isPlaying: Bool = false

    var body: some View {
        VStack {
            Text(episode.title)
                .foregroundStyle(isPlaying ? .primary : .secondary)
            PlayButton(isPlaying: $isPlaying)
        }
    }
}
```

## See Also

### Getting the value

var wrappedValue: Value

The underlying value referenced by the state variable.

