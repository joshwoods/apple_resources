

- Foundation
- NSString
-  components(separatedBy:) 

Instance Method

# components(separatedBy:)

Returns an array containing substrings from the receiver that have been divided by characters in a given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func components(separatedBy separator: CharacterSet) -> [String]
```

## Parameters 

`separator`  

A character set containing the characters to use to split the receiver. Must not be `nil`.

## Return Value

An `NSArray` object containing substrings from the receiver that have been divided by characters in `separator`.

## Discussion

The substrings in the array appear in the order they did in the receiver. Adjacent occurrences of the separator characters produce empty strings in the result. Similarly, if the string begins or ends with separator characters, the first or last substring, respectively, is empty.

## See Also

### Dividing Strings

func components(separatedBy: String) -> [String]

Returns an array containing substrings from the receiver that have been divided by a given separator.

func trimmingCharacters(in: CharacterSet) -> String

Returns a new string made by removing from both ends of the receiver characters contained in a given character set.

func substring(from: Int) -> String

Returns a new string containing the characters of the receiver from the one at a given index to the end.

func substring(with: NSRange) -> String

Returns a string object containing the characters of the receiver that lie within a given range.

func substring(to: Int) -> String

Returns a new string containing the characters of the receiver up to, but not including, the one at a given index.

