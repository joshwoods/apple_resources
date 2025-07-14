

- Foundation
- NSAttributedString
-  textUnfilteredTypes 

Type Property

# textUnfilteredTypes

An array of UTI strings that identify the file types that attributed strings support directly.

macOS 10.5+

``` source
class var textUnfilteredTypes: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains a UTI identifying a supported file type.

## Discussion

The returned list includes UTI strings only for those file types that are supported directly by the receiver. It does not include types that are supported through user-installed filter services. You can use the returned UTI strings with any method that supports UTIs.

## See Also

### Getting the supported text-file formats

func prefersRTFD(in: NSRange) -> Bool

Returns a Boolean value that indicates whether the specified range of text prefers RTFD formatting.

class var textTypes: [String]

An array of UTI strings that identify the file types that attributed strings support, either directly or through a user-installed filter service.

