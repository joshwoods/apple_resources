

- Swift
- Range
-  upToNextMajor(from:) 

Type Method

# upToNextMajor(from:)

Returns a requirement for a version range, starting at the given minimum version and going up to the next major version. This is the recommended version requirement.

macOS 10.10+

``` source
static func upToNextMajor(from version: Version) -> Range where Bound == Version
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`version`  

The minimum version for the version range.

