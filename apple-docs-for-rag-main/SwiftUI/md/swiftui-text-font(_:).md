

- SwiftUI
- Text
-  font(\_:) 

Instance Method

# font(\_:)

Sets the default font for text in the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func font(_ font: Font?) -> Text
```

## Parameters 

`font`  

The font to use when displaying this text.

## Return Value

Text that uses the font you specify.

## Mentioned in 

Applying custom fonts to text

## Discussion

Use `font(_:)` to apply a specific font to an individual Text View, or all of the text views in a container.

In the example below, the first text field has a font set directly, while the font applied to the following container applies to all of the text views inside that container:

```
VStack {
    Text("Font applied to a text view.")
        .font(.largeTitle)

    VStack {
        Text("These two text views have the same font")
        Text("applied to their parent view.")
    }
    .font(.system(size: 16, weight: .light, design: .default))
}
```

## See Also

### Choosing a font

func fontWeight(Font.Weight?) -> Text

Sets the font weight of the text.

func fontDesign(Font.Design?) -> Text

Sets the font design of the text.

func fontWidth(Font.Width?) -> Text

Sets the font width of the text.

