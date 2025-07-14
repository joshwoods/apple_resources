

- SwiftUI
- View
-  fontWidth(\_:) 

Instance Method

# fontWidth(\_:)

Sets the font width of the text in this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func fontWidth(_ width: Font.Width?) -> some View
```

## Parameters 

`width`  

One of the available font widths. Providing `nil` removes the effect of any font width modifier applied higher in the view hierarchy.

## Return Value

A view that uses the font width you specify.

## See Also

### Setting a font

Applying custom fonts to text

Add and use a font in your app that scales with Dynamic Type.

func font(Font?) -> some View

Sets the default font for text in this view.

func fontDesign(Font.Design?) -> some View

Sets the font design of the text in this view.

func fontWeight(Font.Weight?) -> some View

Sets the font weight of the text in this view.

var font: Font?

The default font of this environment.

struct Font

An environment-dependent font.

