

- SwiftUI
- Color
-  init(\_:bundle:) 

Initializer

# init(\_:bundle:)

Creates a color from a color set that you indicate by name.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    _ name: String,
    bundle: Bundle? = nil
)
```

## Parameters 

`name`  

The name of the color resource to look up.

`bundle`  

The bundle in which to search for the color resource. If you don’t indicate a bundle, the initializer looks in your app’s main bundle by default.

## Discussion

Use this initializer to load a color from a color set stored in an Asset Catalog. The system determines which color within the set to use based on the environment at render time. For example, you can provide light and dark versions for background and foreground colors:

You can then instantiate colors by referencing the names of the assets:

```
struct Hello: View {
    var body: some View {
        ZStack {
            Color("background")
            Text("Hello, world!")
                .foregroundStyle(Color("foreground"))
        }
        .frame(width: 200, height: 100)
    }
}
```

SwiftUI renders the appropriate colors for each appearance:

## See Also

### Creating a color

init(_:)

Creates a constant color with the values specified by the resolved color.

func resolve(in: EnvironmentValues) -> Color.Resolved

Evaluates this color to a resolved color given the current `context`.

