

- Foundation
- Scanner
-  scanUpTo(\_:into:) Deprecated

Instance Method

# scanUpTo(\_:into:)

Scans the string until a given string is encountered, accumulating characters into a string that’s returned by reference.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
func scanUpTo(
    _ string: String,
    into result: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`string`  

The string to scan up to.

`result`  

Upon return, contains any characters that were scanned.

## Return Value

true if the receiver scans any characters, otherwise false.

If the only scanned characters are in the charactersToBeSkipped character set (which by default is the whitespace and newline character set), then this method returns false.

## Discussion

If `stopString` is present in the receiver, then on return the scan location is set to the beginning of that string.

If `stopString` is the first string in the receiver, then the method returns false and `stringValue` is not changed.

If the search string (`stopString`) isn’t present in the scanner’s source string, the remainder of the source string is put into `stringValue`, the receiver’s `scanLocation` is advanced to the end of the source string, and the method returns true.

Invoke this method with `NULL` as `stringValue` to simply scan up to a given string.

## See Also

### Scanning Characters and Strings

func scanCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string as long as characters from a given character set are encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanUpToCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a character from a given character set is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanString(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans a given string, returning an equivalent string object by reference if a match is found.

Deprecated

