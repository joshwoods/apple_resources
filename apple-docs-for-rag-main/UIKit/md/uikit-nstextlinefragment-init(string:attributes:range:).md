

- UIKit
- NSTextLineFragment
-  init(string:attributes:range:) 

Initializer

# init(string:attributes:range:)

Creates a new line fragment using the string, attributes, and range you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init(
    string: String,
    attributes: [NSAttributedString.Key : Any] = [:],
    range: NSRange
)
```

## Parameters 

`string`  

An attributed string.

`attributes`  

A dictionary of attributes.

`range`  

The range to use from `string`.

## See Also

### Creating line fragments

init(attributedString: NSAttributedString, range: NSRange)

Creates a new line fragment from the attributed string for the range of characters you specify.

init?(coder: NSCoder)

Creates a new line fragment with from data in an unarchiver.

