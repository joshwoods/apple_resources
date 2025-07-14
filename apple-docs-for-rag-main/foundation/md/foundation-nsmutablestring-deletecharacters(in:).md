

- Foundation
- NSMutableString
-  deleteCharacters(in:) 

Instance Method

# deleteCharacters(in:)

Removes from the receiver the characters in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deleteCharacters(in range: NSRange)
```

## Parameters 

`range`  

The range of characters to delete. `range` must not exceed the bounds of the receiver.

Important

Raises an `NSRangeException` if any part of `range` lies beyond the end of the string.

## Discussion

This method treats the length of the string as a valid range value that returns an empty string.

## See Also

### Modifying a String

func append(String)

Adds to the end of the receiver the characters of a given string.

func applyTransform(StringTransform, reverse: Bool, range: NSRange, updatedRange: NSRangePointer?) -> Bool

Transliterates the receiver by applying a specified ICU string transform.

func insert(String, at: Int)

Inserts into the receiver the characters of a given string at a given location.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters from `range` with those in `aString`.

func replaceOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> Int

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

func setString(String)

Replaces the characters of the receiver with those in a given string.

