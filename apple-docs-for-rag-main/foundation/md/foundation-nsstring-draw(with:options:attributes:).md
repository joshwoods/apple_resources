

- Foundation
- NSString
-  draw(with:options:attributes:) 

Instance Method

# draw(with:options:attributes:)

Draws the receiver with the specified options and other display characteristics of the given attributes, within the specified rectangle in the current graphics context.

macOS 10.0+

``` source
func draw(
    with rect: NSRect,
    options: NSString.DrawingOptions = [],
    attributes: [NSAttributedString.Key : Any]? = nil
)
```

## Parameters 

`rect`  

The rectangle in which to draw the string.

`options`  

String drawing options.

`attributes`  

A dictionary of text attributes to be applied to the string. These are the same attributes that can be applied to an `NSAttributedString` object, but in the case of `NSString` objects, the attributes apply to the entire string, rather than ranges within the string.

## Discussion

This method works in single-line, baseline rendering configuration by default. That is, the `rect` argument’s `origin` field specifies the rendering origin, and that point is interpreted as the baseline origin by default. If the string drawing option `NSStringDrawingUsesLineFragmentOrigin` is specified, `origin` is interpreted as the upper left corner of the line fragment rectangle, and the method behaves in multiline configuration.

The `size` field specifies the text container size. The `width` part of the size field specifies the maximum line fragment width if larger than `0.0`. The `height` defines the maximum size that can be occupied with text if larger than `0.0` and `NSStringDrawingUsesLineFragmentOrigin` is specified. If `NSStringDrawingUsesLineFragmentOrigin` is not specified, height is ignored and considered to be single-line rendering (`NSLineBreakByWordWrapping` and `NSLineBreakByCharWrapping` are treated as `NSLineBreakByClipping`).

You should only invoke this method when there is a current graphics context.

## See Also

### Deprecated

class func string(withCString: UnsafePointer&lt;CChar>) -> Any?

Creates a new string using a given C-string.

Deprecated

convenience init?(CString: UnsafePointer&lt;CChar>)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

class func string(withCString: UnsafePointer&lt;CChar>, length: Int) -> Any?

Returns a string containing the characters in a given C-string.

Deprecated

convenience init?(CString: UnsafePointer&lt;CChar>, length: Int)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

convenience init?(CStringNoCopy: UnsafeMutablePointer&lt;CChar>, length: Int, freeWhenDone: Bool)

Initializes the receiver, a newly allocated `NSString` object, by converting the data in a given C-string from the default C-string encoding into the Unicode character encoding.

Deprecated

class func string(withContentsOfFile: String) -> Any?

Returns a string created by reading data from the file named by a given path.

Deprecated

convenience init?(contentsOfFile: String)

Initializes the receiver, a newly allocated `NSString` object, by reading data from the file named by `path`.

Deprecated

class func string(withContentsOf: URL) -> Any?

Returns a string created by reading data from the file named by a given URL.

Deprecated

convenience init?(contentsOfURL: URL)

Initializes the receiver, a newly allocated `NSString` object, by reading data from the location named by a given URL.

Deprecated

func write(toFile: String, atomically: Bool) -> Bool

Writes the contents of the receiver to the file specified by a given path.

Deprecated

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the receiver to the location specified by a given URL.

Deprecated

func getCharacters(UnsafeMutablePointer&lt;unichar>)

Copies all characters from the receiver into a given buffer.

Deprecated

func cString() -> UnsafePointer&lt;CChar>?

Returns a representation of the receiver as a C string in the default C-string encoding.

Deprecated

func lossyCString() -> UnsafePointer&lt;CChar>?

Returns a representation of the receiver as a C string in the default C-string encoding, possibly losing information in converting to that encoding.

Deprecated

func cStringLength() -> Int

Returns the length in char-sized units of the receiver’s C-string representation in the default C-string encoding.

Deprecated

