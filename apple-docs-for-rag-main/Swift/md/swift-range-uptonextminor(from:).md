

- Swift
- Range
-  upToNextMinor(from:) 

Type Method

# upToNextMinor(from:)

Returns a requirement for a version range, starting at the given minimum version and going up to the next minor version.

macOS 10.10+

``` source
static func upToNextMinor(from version: Version) -> Range where Bound == Version
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`version`  

The minimum version for the version range.

