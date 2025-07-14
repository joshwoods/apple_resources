

- PDFKit
- PDFPage
-  characterIndex(at:) 

Instance Method

# characterIndex(at:)

Returns the character index value for the specified point in page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func characterIndex(at point: CGPoint) -> Int
```

**macOS**

``` source
func characterIndex(at point: NSPoint) -> Int
```

## Discussion

If there is no character at the specified point, the method returns `-1`.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Working with Textual Content

var numberOfCharacters: Int

Returns the number of characters on the page, including whitespace characters.

var string: String?

Returns an `NSString` object representing the text on the page.

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text on the page.

func characterBounds(at: Int) -> CGRect

Returns the bounds, in page space, of the character at the specified index.

