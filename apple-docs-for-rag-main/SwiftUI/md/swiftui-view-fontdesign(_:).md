

- SwiftUI
- View
-  fontDesign(\_:) 

Instance Method

# fontDesign(\_:)

Sets the font design of the text in this view.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
nonisolated
func fontDesign(_ design: Font.Design?) -> some View
```

## Parameters 

`design`  

One of the available font designs. Providing `nil` removes the effect of any font design modifier applied higher in the view hierarchy.

## Return Value

A view that uses the font design you specify.

## See Also

### Setting a font

Applying custom fonts to text

Add and use a font in your app that scales with Dynamic Type.

func font(Font?) -> some View

Sets the default font for text in this view.

func fontWeight(Font.Weight?) -> some View

Sets the font weight of the text in this view.

func fontWidth(Font.Width?) -> some View

Sets the font width of the text in this view.

var font: Font?

The default font of this environment.

struct Font

An environment-dependent font.

