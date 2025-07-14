

- Foundation
- Scanner
-  scanUpToCharacters(from:into:) Deprecated

Instance Method

# scanUpToCharacters(from:into:)

Scans the string until a character from a given character set is encountered, accumulating characters into a string that’s returned by reference.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
func scanUpToCharacters(
    from set: CharacterSet,
    into result: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`set`  

The set of characters up to which to scan.

`result`  

Upon return, contains the characters scanned.

## Return Value

true if the receiver scanned any characters, otherwise false.

If the only scanned characters are in the charactersToBeSkipped character set (which is the whitespace and newline character set by default), then returns false.

## Discussion

Invoke this method with `NULL` as `stringValue` to simply scan up to a given set of characters.

If no characters in `stopSet` are present in the scanner’s source string, the remainder of the source string is put into `stringValue`, the receiver’s `scanLocation` is advanced to the end of the source string, and the method returns true.

## See Also

### Scanning Characters and Strings

func scanCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string as long as characters from a given character set are encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanString(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans a given string, returning an equivalent string object by reference if a match is found.

Deprecated

func scanUpTo(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a given string is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

