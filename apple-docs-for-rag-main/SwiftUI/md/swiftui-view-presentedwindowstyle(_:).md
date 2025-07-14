

- SwiftUI
- View
-  presentedWindowStyle(\_:) 

Instance Method

# presentedWindowStyle(\_:)

Sets the style for windows created by interacting with this view.

macOS 11.0+

``` source
nonisolated
func presentedWindowStyle(_ style: S) -> some View where S : WindowStyle
```

## See Also

### Styling windows from a view inside the window

func presentedWindowToolbarStyle&lt;S>(S) -> some View

Sets the style for the toolbar in windows created by interacting with this view.

