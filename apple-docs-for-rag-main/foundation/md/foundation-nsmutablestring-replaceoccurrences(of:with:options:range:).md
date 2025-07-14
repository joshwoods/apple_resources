

- Foundation
- NSMutableString
-  replaceOccurrences(of:with:options:range:) 

Instance Method

# replaceOccurrences(of:with:options:range:)

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceOccurrences(
    of target: String,
    with replacement: String,
    options: NSString.CompareOptions = [],
    range searchRange: NSRange
) -> Int
```

## Parameters 

`target`  

The string to replace.

Important

Raises an `NSInvalidArgumentException` if `target` is `nil`.

`replacement`  

The string with which to replace `target`.

Important

Raises an `NSInvalidArgumentException` if `replacement` is `nil`.

`options`  

A mask specifying search options. See String Programming Guide for details.

If `opts` is `NSBackwardsSearch`, the search is done from the end of the range. If `opts` is `NSAnchoredSearch`, only anchored (but potentially multiple) instances are replaced. `NSLiteralSearch` and `NSCaseInsensitiveSearch` also apply.

`searchRange`  

The range of characters to replace. `searchRange` must not exceed the bounds of the receiver. Specify `searchRange` as `NSMakeRange(0, [receiver length])` to process the entire string.

Important

Raises an `NSRangeException` if any part of `searchRange` lies beyond the end of the receiver.

## Return Value

The number of replacements made.

## Discussion

This method treats the length of the string as a valid range value that returns an empty string.

## See Also

### Modifying a String

func append(String)

Adds to the end of the receiver the characters of a given string.

func applyTransform(StringTransform, reverse: Bool, range: NSRange, updatedRange: NSRangePointer?) -> Bool

Transliterates the receiver by applying a specified ICU string transform.

func deleteCharacters(in: NSRange)

Removes from the receiver the characters in a given range.

func insert(String, at: Int)

Inserts into the receiver the characters of a given string at a given location.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters from `range` with those in `aString`.

func setString(String)

Replaces the characters of the receiver with those in a given string.

