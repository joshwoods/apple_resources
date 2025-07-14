

- Foundation
- NSTextCheckingResult
-  orthography 

Instance Property

# orthography

The detected orthography of a type checking result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var orthography: NSOrthography? { get }
```

## See Also

### Text Checking Results for Orthography

class func orthographyCheckingResult(range: NSRange, orthography: NSOrthography) -> NSTextCheckingResult

Creates and returns a text checking result with the specified orthography.

