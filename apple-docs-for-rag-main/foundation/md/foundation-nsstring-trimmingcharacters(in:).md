

- Foundation
- NSString
-  trimmingCharacters(in:) 

Instance Method

# trimmingCharacters(in:)

Returns a new string made by removing from both ends of the receiver characters contained in a given character set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func trimmingCharacters(in set: CharacterSet) -> String
```

## Parameters 

`set`  

A character set containing the characters to remove from the receiver. `set` must not be `nil`.

## Return Value

A new string made by removing from both ends of the receiver characters contained in `set`. If the receiver is composed entirely of characters from `set`, the empty string is returned.

## Discussion

Use whitespaces or whitespacesAndNewlines to remove whitespace around strings.

## See Also

### Dividing Strings

func components(separatedBy: String) -> [String]

Returns an array containing substrings from the receiver that have been divided by a given separator.

func components(separatedBy: CharacterSet) -> [String]

Returns an array containing substrings from the receiver that have been divided by characters in a given set.

func substring(from: Int) -> String

Returns a new string containing the characters of the receiver from the one at a given index to the end.

func substring(with: NSRange) -> String

Returns a string object containing the characters of the receiver that lie within a given range.

func substring(to: Int) -> String

Returns a new string containing the characters of the receiver up to, but not including, the one at a given index.

