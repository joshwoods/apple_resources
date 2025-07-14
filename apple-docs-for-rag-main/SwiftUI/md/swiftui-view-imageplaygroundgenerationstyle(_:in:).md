

- SwiftUI
- View
-  imagePlaygroundGenerationStyle(\_:in:) 

Instance Method

# imagePlaygroundGenerationStyle(\_:in:)

Sets the generation style for an image playground.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
nonisolated
func imagePlaygroundGenerationStyle(
    _ style: ImagePlaygroundStyle,
    in allowedStyles: [ImagePlaygroundStyle] = ImagePlaygroundStyle.all
) -> some View
```

## Parameters 

`style`  

The generation style that the playground uses.

`allowedStyles`  

The list of generation styles that the `style` input can have. Use `ImagePlaygroundStyle.all` to check the list of all possible styles, and pass a subset of those.

## Return Value

An image playground sheet that uses one of the specified generation `styles`.

