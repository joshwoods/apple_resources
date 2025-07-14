

- SwiftUI
- Binding
-  projectedValue 

Instance Property

# projectedValue

A projection of the binding value that returns a binding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var projectedValue: Binding { get }
```

## Discussion

Use the projected value to pass a binding value down a view hierarchy. To get the `projectedValue`, prefix the property variable with `$`. For example, in the following code example `PlayerView` projects a binding of the state property `isPlaying` to the `PlayButton` view using `$isPlaying`.

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

The underlying value referenced by the binding variable.

subscript&lt;Subject>(dynamicMember _: WritableKeyPath&lt;Value, Subject>) -> Binding&lt;Subject>

Returns a binding to the resulting value of a given key path.

