

- RealityKit
- Model3DPlaceholderContent
-  listItemTint(\_:) 

Instance Method

# listItemTint(\_:)

Sets the tint effect for content in a list.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func listItemTint(_ tint: ListItemTint?) -> some View
```

## Parameters 

`tint`  

The tint effect to use. Use `nil` to avoid overriding the inherited tint.

## Discussion

The containing list’s style applies the tint as appropriate. For example, watchOS uses the tint color for its background platter appearance. Sidebars on iOS and macOS apply the tint color to their `Label` icons, which otherwise use the accent color by default.

