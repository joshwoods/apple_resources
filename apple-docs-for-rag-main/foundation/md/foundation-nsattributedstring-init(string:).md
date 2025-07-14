

- Foundation
- NSAttributedString
-  init(string:) 

Initializer

# init(string:)

Creates an attributed string with the specified text and no attribute information.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(string str: String)
```

## Parameters 

`str`  

The text for the new attributed string.

## Return Value

An NSAttributedString object initialized with the characters of `str` and no attribute information.

## See Also

### Related Documentation

init?(RTF: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

Attributed String Programming Guide

### Creating from another string

init(string: String, attributes: [NSAttributedString.Key : Any]?)

Creates an attributed string with the specified text and attributes.

init(attributedString: NSAttributedString)

Creates a new attributed string from the contents of another attributed string.

