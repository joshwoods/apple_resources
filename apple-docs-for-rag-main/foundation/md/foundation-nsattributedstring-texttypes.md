

- Foundation
- NSAttributedString
-  textTypes 

Type Property

# textTypes

An array of UTI strings that identify the file types that attributed strings support, either directly or through a user-installed filter service.

macOS 10.5+

``` source
class var textTypes: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains a UTI identifying a supported file type.

## Discussion

The returned list includes UTIs all file types supported by the receiver plus those that can be opened by the receiver after being converted by a user-installed filter service. You can use the returned UTI strings with any method that supports UTIs.

## See Also

### Getting the supported text-file formats

func prefersRTFD(in: NSRange) -> Bool

Returns a Boolean value that indicates whether the specified range of text prefers RTFD formatting.

class var textUnfilteredTypes: [String]

An array of UTI strings that identify the file types that attributed strings support directly.

