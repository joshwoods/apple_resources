

- Foundation
- NSMutableString
-  applyTransform(\_:reverse:range:updatedRange:) 

Instance Method

# applyTransform(\_:reverse:range:updatedRange:)

Transliterates the receiver by applying a specified ICU string transform.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func applyTransform(
    _ transform: StringTransform,
    reverse: Bool,
    range: NSRange,
    updatedRange resultingRange: NSRangePointer?
) -> Bool
```

## Parameters 

`transform`  

The transformation to apply. For a list of possible values, see String Transformations. If the specified transform does not exist, the receiver is not modified, and this method returns false.

`reverse`  

Whether an inverse transform should be used. If the specified transform does not have an inverse, the receiver is not modified, and this method returns false.

`range`  

The range of the string to transform. `range` must not exceed the bounds of the receiver.

Important

Raises an `NSRangeException` if any part of `aRange` lies beyond the end of the string.

`resultingRange`  

If the transform was successfully applied, upon return contains the range of the transformed string.

## Return Value

true if the transform was successfully applied. Otherwise, false.

## Discussion

In addition to the provided transformation constants, you may use any valid ICU transform ID as defined in the ICU User Guide. However, arbitrary ICU transform rules are not supported.

## See Also

### Modifying a String

func append(String)

Adds to the end of the receiver the characters of a given string.

func deleteCharacters(in: NSRange)

Removes from the receiver the characters in a given range.

func insert(String, at: Int)

Inserts into the receiver the characters of a given string at a given location.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters from `range` with those in `aString`.

func replaceOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> Int

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

func setString(String)

Replaces the characters of the receiver with those in a given string.

