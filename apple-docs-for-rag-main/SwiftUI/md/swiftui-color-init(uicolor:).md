

- SwiftUI
- Color
-  init(uiColor:) 

Initializer

# init(uiColor:)

Creates a color from a UIKit color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(uiColor: UIColor)
```

## Discussion

Use this method to create a SwiftUI color from a UIColor instance. The new color preserves the adaptability of the original. For example, you can create a rectangle using link to see how the shade adjusts to match the user’s system settings:

```
struct Box: View {
    var body: some View {
        Color(uiColor: .link)
            .frame(width: 200, height: 100)
    }
}
```

The `Box` view defined above automatically changes its appearance when the user turns on Dark Mode. With the light and dark appearances placed side by side, you can see the subtle difference in shades:

Note

Use this initializer only if you need to convert an existing UIColor to a SwiftUI color. Otherwise, create a SwiftUI Color using an initializer like init(_:red:green:blue:opacity:), or use a system color like blue.

## See Also

### Creating a color from another color

init(nsColor: NSColor)

Creates a color from an AppKit color.

init(cgColor: CGColor)

Creates a color from a Core Graphics color.

