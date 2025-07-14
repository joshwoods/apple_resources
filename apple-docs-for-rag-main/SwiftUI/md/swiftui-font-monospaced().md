

- SwiftUI
- Font
-  monospaced() 

Instance Method

# monospaced()

Returns a fixed-width font from the same family as the base font.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func monospaced() -> Font
```

## Return Value

A fixed-width font from the same family as the base font, if one is available, and a default fixed-width font otherwise.

## Discussion

If there’s no suitable font face in the same family, SwiftUI returns a default fixed-width font.

The following example adds the `monospaced()` modifier to the default system font, then applies this font to a Text view:

```
struct ContentView: View {
    let myFont = Font
        .system(size: 24)
        .monospaced()

    var body: some View {
        Text("Hello, world!")
            .font(myFont)
            .padding()
            .navigationTitle("Monospaced")
    }
}
```

SwiftUI may provide different fixed-width replacements for standard user interface fonts (such as title, or a system font created with system(_:design:)) than for those same fonts when created by name with custom(_:size:).

The font(_:) modifier applies the font to all text within the view. To mix fixed-width text with other styles in the same `Text` view, use the init(_:) initializer to use an appropropriately-styled AttributedString for the text view’s content. You can use the init(markdown:options:baseURL:) initializer to provide a Markdown-formatted string containing the backtick-syntax (\`…\`) to apply code voice to specific ranges of the attributed string.

## See Also

### Styling a font

func bold() -> Font

Adds bold styling to the font.

func italic() -> Font

Adds italics to the font.

func monospacedDigit() -> Font

Returns a modified font that uses fixed-width digits, while leaving other characters proportionally spaced.

func smallCaps() -> Font

Adjusts the font to enable all small capitals.

func lowercaseSmallCaps() -> Font

Adjusts the font to enable lowercase small capitals.

func uppercaseSmallCaps() -> Font

Adjusts the font to enable uppercase small capitals.

func weight(Font.Weight) -> Font

Sets the weight of the font.

func width(Font.Width) -> Font

Sets the width of the font.

struct Width

A width to use for fonts that have multiple widths.

func leading(Font.Leading) -> Font

Adjusts the line spacing of a font.

enum Leading

A line spacing adjustment that you can apply to a font.

