

- Foundation
- NSAttributedString
-  init(attributedString:) 

Initializer

# init(attributedString:)

Creates a new attributed string from the contents of another attributed string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(attributedString attrStr: NSAttributedString)
```

## Parameters 

`attrStr`  

An attributed string.

## Return Value

An NSAttributedString object initialized with the characters and attributes of `attrStr`.

## See Also

### Related Documentation

init?(RTF: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

### Creating from another string

init(string: String)

Creates an attributed string with the specified text and no attribute information.

init(string: String, attributes: [NSAttributedString.Key : Any]?)

Creates an attributed string with the specified text and attributes.

