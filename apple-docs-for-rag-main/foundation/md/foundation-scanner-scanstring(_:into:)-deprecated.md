

- Foundation
- Scanner
-  scanString(\_:into:) Deprecated

Instance Method

# scanString(\_:into:)

Scans a given string, returning an equivalent string object by reference if a match is found.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
func scanString(
    _ string: String,
    into result: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`string`  

The string for which to scan at the current scan location.

`result`  

Upon return, if the receiver contains a string equivalent to `string` at the current scan location, contains a string equivalent to `string`.

## Return Value

true if `string` matches the characters at the scan location, otherwise false.

## Discussion

If `string` is present at the current scan location, then the current scan location is advanced to after the string; otherwise the scan location does not change.

Invoke this method with `NULL` as `stringValue` to simply scan past a given string.

## See Also

### Scanning Characters and Strings

func scanCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string as long as characters from a given character set are encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanUpToCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a character from a given character set is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanUpTo(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a given string is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

