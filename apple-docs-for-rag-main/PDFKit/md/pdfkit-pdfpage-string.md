

- PDFKit
- PDFPage
-  string 

Instance Property

# string

Returns an `NSString` object representing the text on the page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var string: String? { get }
```

## See Also

### Working with Textual Content

var numberOfCharacters: Int

Returns the number of characters on the page, including whitespace characters.

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text on the page.

func characterBounds(at: Int) -> CGRect

Returns the bounds, in page space, of the character at the specified index.

func characterIndex(at: CGPoint) -> Int

Returns the character index value for the specified point in page space.

