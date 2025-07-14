

- Foundation
- NSAttributedString
-  attributedSubstring(from:) 

Instance Method

# attributedSubstring(from:)

Returns an attributed string consisting of the characters and attributes within the specified range in the attributed string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attributedSubstring(from range: NSRange) -> NSAttributedString
```

## Parameters 

`range`  

The range from which to create a new attributed string. `aRange` must lie within the bounds of the receiver.

## Return Value

An `NSAttributedString` object consisting of the characters and attributes within `aRange` in the receiver.

## Discussion

Raises an rangeException if any part of `aRange` lies beyond the end of the receiver’s characters. This method treats the length of the string as a valid range value that returns an empty string.

## See Also

### Getting the characters

var string: String

The character contents of the attributed string as a string.

var length: Int

The length of the attributed string.

