

- Foundation
- NSString
-  appending(\_:) 

Instance Method

# appending(\_:)

Returns a new string made by appending a given string to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func appending(_ aString: String) -> String
```

## Parameters 

`aString`  

The string to append to the receiver. This value must not be `nil`.

Important

Raises an `NSInvalidArgumentException` if `aString` is `nil`.

## Return Value

A new string made by appending `aString` to the receiver.

## Discussion

This code excerpt, for example:

```
NSString *errorTag = @"Error: ";
NSString *errorString = @"premature end of file.";
NSString *errorMessage = [errorTag stringByAppendingString:errorString];
```

produces the string “`Error: premature end of file.`”.

## See Also

### Combining Strings

func appendingFormat(NSString, any CVarArg...) -> NSString

func padding(toLength: Int, withPad: String, startingAt: Int) -> String

Returns a new string formed from the receiver by either removing characters from the end, or by appending as many occurrences as necessary of a given pad string.

