

- Foundation
- NSMutableString
-  setString(\_:) 

Instance Method

# setString(\_:)

Replaces the characters of the receiver with those in a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setString(_ aString: String)
```

## Parameters 

`aString`  

The string with which to replace the receiver’s content. `aString` must not be `nil`.

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

func replaceOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> Int

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

