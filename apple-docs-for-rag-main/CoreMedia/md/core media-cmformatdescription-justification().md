

- Core Media
- CMFormatDescription
-  justification() 

Instance Method

# justification()

Returns the horizontal and vertical justification.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func justification() throws -> (horizontal: CMFormatDescription.Extensions.Value.TextJustification, vertical: CMFormatDescription.Extensions.Value.TextJustification)
```

## See Also

### Working with Text Descriptions

func defaultStyle() throws -> (localFontID: Int, bold: Bool, italic: Bool, underline: Bool, fontSize: CGFloat, colorComponents: [CGFloat])

Returns the default text style.

func defaultTextBox(originIsAtTopLeft: Bool, heightOfTextTrack: CGFloat) throws -> CGRect

Returns the default text box.

func displayFlags() throws -> CMFormatDescription.Extensions.Value.TextDisplayFlags

Returns the display mode flags for the text media.

func fontName(localFontID: Int) throws -> String

Returns the font name for the local font identifier.

