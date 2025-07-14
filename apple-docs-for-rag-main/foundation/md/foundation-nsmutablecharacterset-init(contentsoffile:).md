

- Foundation
- NSMutableCharacterSet
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Returns a character set read from the bitmap representation stored in the file a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(contentsOfFile fName: String)
```

## See Also

### Creating Custom Character Sets

init(charactersIn: String)

Returns a character set containing the characters in a given string.

init(range: NSRange)

Returns a character set containing characters with Unicode values in a given range.

init(bitmapRepresentation: Data)

Returns a character set containing characters determined by a given bitmap representation.

