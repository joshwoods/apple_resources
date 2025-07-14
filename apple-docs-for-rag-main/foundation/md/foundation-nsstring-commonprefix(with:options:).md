

- Foundation
- NSString
-  commonPrefix(with:options:) 

Instance Method

# commonPrefix(with:options:)

Returns a string containing characters the receiver and a given string have in common, starting from the beginning of each up to the first characters that aren’t equivalent.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func commonPrefix(
    with str: String,
    options mask: NSString.CompareOptions = []
) -> String
```

## Parameters 

`str`  

The string with which to compare the receiver.

`mask`  

Options for the comparison. The following search options may be specified by combining them with the C bitwise `OR` operator: `NSCaseInsensitiveSearch`, `NSLiteralSearch`. See String Programming Guide for details on these options.

## Return Value

A string containing characters the receiver and `aString` have in common, starting from the beginning of each up to the first characters that aren’t equivalent.

## Discussion

The returned string is based on the characters of the receiver. For example, if the receiver is “Ma¨dchen” and `aString` is “Mädchenschule”, the string returned is “Ma¨dchen”, not “Mädchen”.

## See Also

### Related Documentation

func hasPrefix(String) -> Bool

Returns a Boolean value that indicates whether a given string matches the beginning characters of the receiver.

