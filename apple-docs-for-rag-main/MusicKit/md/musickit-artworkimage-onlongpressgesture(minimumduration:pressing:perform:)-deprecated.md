

- MusicKit
- ArtworkImage
-  onLongPressGesture(minimumDuration:pressing:perform:) Deprecated

Instance Method

# onLongPressGesture(minimumDuration:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

MusicKitSwiftUItvOS 14.0–18.4Deprecated

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

