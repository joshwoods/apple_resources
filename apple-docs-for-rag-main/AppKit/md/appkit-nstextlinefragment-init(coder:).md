

- AppKit
- NSTextLineFragment
-  init(coder:) 

Initializer

# init(coder:)

Creates a new line fragment with from data in an unarchiver.

macOS 12.0+

``` source
init?(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

A decoder that conforms to the NSCoder protocol.

## See Also

### Creating line fragments

init(attributedString: NSAttributedString, range: NSRange)

Creates a new line fragment from the attributed string for the range of characters you specify.

convenience init(string: String, attributes: [NSAttributedString.Key : Any], range: NSRange)

Creates a new line fragment using the string, attributes, and range you provide.

