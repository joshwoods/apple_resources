

- AppKit
- NSTextLineFragment
-  init(attributedString:range:) 

Initializer

# init(attributedString:range:)

Creates a new line fragment from the attributed string for the range of characters you specify.

macOS 12.0+

``` source
init(
    attributedString: NSAttributedString,
    range: NSRange
)
```

## Parameters 

`attributedString`  

The attributed string.

`range`  

An NSRange that specifies which characters to include.

## See Also

### Creating line fragments

init?(coder: NSCoder)

Creates a new line fragment with from data in an unarchiver.

convenience init(string: String, attributes: [NSAttributedString.Key : Any], range: NSRange)

Creates a new line fragment using the string, attributes, and range you provide.

