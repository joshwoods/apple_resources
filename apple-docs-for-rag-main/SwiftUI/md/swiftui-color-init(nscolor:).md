

- SwiftUI
- Color
-  init(nsColor:) 

Initializer

# init(nsColor:)

Creates a color from an AppKit color.

macOS 12.0+

``` source
nonisolated
init(nsColor: NSColor)
```

## Discussion

Use this method to create a SwiftUI color from an NSColor instance. The new color preserves the adaptability of the original. For example, you can create a rectangle using linkColor to see how the shade adjusts to match the user’s system settings:

```
struct Box: View {
    var body: some View {
        Color(nsColor: .linkColor)
            .frame(width: 200, height: 100)
    }
}
```

The `Box` view defined above automatically changes its appearance when the user turns on Dark Mode. With the light and dark appearances placed side by side, you can see the subtle difference in shades:

Note

Use this initializer only if you need to convert an existing NSColor to a SwiftUI color. Otherwise, create a SwiftUI Color using an initializer like init(_:red:green:blue:opacity:), or use a system color like blue.

## See Also

### Creating a color from another color

init(uiColor: UIColor)

Creates a color from a UIKit color.

init(cgColor: CGColor)

Creates a color from a Core Graphics color.

