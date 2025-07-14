

- Foundation
- NSMutableString
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts into the receiver the characters of a given string at a given location.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func insert(
    _ aString: String,
    at loc: Int
)
```

## Parameters 

`aString`  

The string to insert into the receiver. `aString` must not be `nil`.

`loc`  

The location at which `aString` is inserted. The location must not exceed the bounds of the receiver.

Important

Raises an `NSRangeException` if `loc` lies beyond the end of the string.

## Discussion

The new characters begin at `loc` and the existing characters from `loc` to the end are shifted by the length of `aString`.

This method treats the length of the string as a valid index value that returns an empty string.

## See Also

### Modifying a String

func append(String)

Adds to the end of the receiver the characters of a given string.

func applyTransform(StringTransform, reverse: Bool, range: NSRange, updatedRange: NSRangePointer?) -> Bool

Transliterates the receiver by applying a specified ICU string transform.

func deleteCharacters(in: NSRange)

Removes from the receiver the characters in a given range.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters from `range` with those in `aString`.

func replaceOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> Int

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

func setString(String)

Replaces the characters of the receiver with those in a given string.

