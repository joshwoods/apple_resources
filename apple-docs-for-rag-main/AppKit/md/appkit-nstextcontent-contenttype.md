

- AppKit
- NSTextContent
-  contentType 

Instance Property

# contentType

The semantic meaning for a text input area.

macOS 11.0+

``` source
var contentType: NSTextContentType? { get set }
```

**Required**

## Discussion

Use this property to give the system information about the expected semantic meaning for the content that people enter. For example, you might specify emailAddress for a text field that people fill in to receive an email confirmation.

For possible values you can use, see NSTextContentType; by default, the value of this property is `nil`.

## See Also

### Specifying content type

struct NSTextContentType

Constants that identify the semantic meaning for a text-entry area.

