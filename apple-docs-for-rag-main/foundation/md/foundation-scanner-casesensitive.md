

- Foundation
- Scanner
-  caseSensitive 

Instance Property

# caseSensitive

Flag that indicates whether the receiver distinguishes case in the characters it scans.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var caseSensitive: Bool { get set }
```

## Discussion

true if the receiver distinguishes case in the characters it scans, otherwise false. The default value is false. Note that case sensitivity doesn’t apply to the characters to be skipped.

## See Also

### Configuring a Scanner

var scanLocation: Int

The character position at which the receiver will begin its next scanning operation.

Deprecated

var charactersToBeSkipped: CharacterSet?

Character set containing the characters the scanner ignores when looking for a scannable element.

var locale: Any?

The locale to use when scanning.

