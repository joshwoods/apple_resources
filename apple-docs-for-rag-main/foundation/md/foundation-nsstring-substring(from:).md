

- Foundation
- NSString
-  substring(from:) 

Instance Method

# substring(from:)

Returns a new string containing the characters of the receiver from the one at a given index to the end.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func substring(from: Int) -> String
```

## Parameters 

`from`  

An index. The value must lie within the bounds of the receiver, or be equal to the length of the receiver.

Raises an rangeException if (`anIndex` - 1) lies beyond the end of the receiver.

## Return Value

A new string containing the characters of the receiver from the one at `anIndex` to the end. If `anIndex` is equal to the length of the string, returns an empty string.

## See Also

### Dividing Strings

func components(separatedBy: String) -> [String]

Returns an array containing substrings from the receiver that have been divided by a given separator.

func components(separatedBy: CharacterSet) -> [String]

Returns an array containing substrings from the receiver that have been divided by characters in a given set.

func trimmingCharacters(in: CharacterSet) -> String

Returns a new string made by removing from both ends of the receiver characters contained in a given character set.

func substring(with: NSRange) -> String

Returns a string object containing the characters of the receiver that lie within a given range.

func substring(to: Int) -> String

Returns a new string containing the characters of the receiver up to, but not including, the one at a given index.

