

- SwiftUI
- View
-  equatable() 

Instance Method

# equatable()

Prevents the view from updating its child view when its new value is the same as its old value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func equatable() -> EquatableView
```

Available when `Self` conforms to `Equatable`.

## See Also

### Managing the view hierarchy

func id&lt;ID>(ID) -> some View

Binds a view’s identity to the given proxy value.

func tag&lt;V>(V, includeOptional: Bool) -> some View

Sets the unique tag value of this view.

