

- Foundation
- NSAttributedString
-  init(string:attributes:) 

Initializer

# init(string:attributes:)

Creates an attributed string with the specified text and attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    string str: String,
    attributes attrs: [NSAttributedString.Key : Any]? = nil
)
```

## Parameters 

`str`  

The text for the new attributed string.

`attrs`  

The attributes for the new attributed string. This method applies the attributes to the entire string. For a list of attributes that you can include in this dictionary, see NSAttributedString.Key.

## Discussion

Returns an NSAttributedString object initialized with the characters of `str` and the attributes of `attrs`.

## See Also

### Related Documentation

init?(RTF: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

### Creating from another string

init(string: String)

Creates an attributed string with the specified text and no attribute information.

init(attributedString: NSAttributedString)

Creates a new attributed string from the contents of another attributed string.

