

- Foundation
- NSString
-  components(separatedBy:) 

Instance Method

# components(separatedBy:)

Returns an array containing substrings from the receiver that have been divided by a given separator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func components(separatedBy separator: String) -> [String]
```

## Parameters 

`separator`  

The separator string.

## Return Value

An `NSArray` object containing substrings from the receiver that have been divided by `separator`.

## Discussion

The substrings in the array appear in the order they did in the receiver. Adjacent occurrences of the separator string produce empty strings in the result. Similarly, if the string begins or ends with the separator, the first or last substring, respectively, is empty. For example, this code fragment:

```
NSString *list = @"Karin, Carrie, David";
NSArray *listItems = [list componentsSeparatedByString:@", "];
```

produces the array `@[@"Karin", @"Carrie", @"David"]`.

If `list` begins with a comma and space—for example, `@", Norman, Stanley, Fletcher"`—the array has these contents: `@[@"", @"Norman", @"Stanley", @"Fletcher"]`.

If `list` has no separators—for example, `@"Karin"`—the array contains the string itself, in this case `@[@"Karin"]`.

## See Also

### Related Documentation

var pathComponents: [String]

The file-system path components of the receiver.

func componentsJoined(by: String) -> String

Constructs and returns an `NSString` object that is the result of interposing a given separator between the elements of the array.

### Dividing Strings

func components(separatedBy: CharacterSet) -> [String]

Returns an array containing substrings from the receiver that have been divided by characters in a given set.

func trimmingCharacters(in: CharacterSet) -> String

Returns a new string made by removing from both ends of the receiver characters contained in a given character set.

func substring(from: Int) -> String

Returns a new string containing the characters of the receiver from the one at a given index to the end.

func substring(with: NSRange) -> String

Returns a string object containing the characters of the receiver that lie within a given range.

func substring(to: Int) -> String

Returns a new string containing the characters of the receiver up to, but not including, the one at a given index.

