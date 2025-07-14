

- PDFKit
- PDFPage
-  characterBounds(at:) 

Instance Method

# characterBounds(at:)

Returns the bounds, in page space, of the character at the specified index.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
func characterBounds(at index: Int) -> NSRect
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func characterBounds(at index: Int) -> CGRect
```

## Discussion

In the unlikely event that there is more than one character at the specified index point, only the bounds of the first character is returned.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page. Note that the bounds returned are not guaranteed to have integer coordinates.

## See Also

### Working with Textual Content

var numberOfCharacters: Int

Returns the number of characters on the page, including whitespace characters.

var string: String?

Returns an `NSString` object representing the text on the page.

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text on the page.

func characterIndex(at: CGPoint) -> Int

Returns the character index value for the specified point in page space.

