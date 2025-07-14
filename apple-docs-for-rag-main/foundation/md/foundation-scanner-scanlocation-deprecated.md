

- Foundation
- Scanner
-  scanLocation Deprecated

Instance Property

# scanLocation

The character position at which the receiver will begin its next scanning operation.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
var scanLocation: Int { get set }
```

## Discussion

Raises an `NSRangeException` if `index` is beyond the end of the string being scanned.

This property is useful for backing up to rescan after an error.

Rather than setting the scan location directly to skip known sequences of characters, use scanString(_:into:) or scanCharacters(from:into:), which allow you to verify that the expected substring (or set of characters) is in fact present.

## See Also

### Configuring a Scanner

var caseSensitive: Bool

Flag that indicates whether the receiver distinguishes case in the characters it scans.

var charactersToBeSkipped: CharacterSet?

Character set containing the characters the scanner ignores when looking for a scannable element.

var locale: Any?

The locale to use when scanning.

