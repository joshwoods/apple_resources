

- Foundation
- NSTextCheckingResult
-  orthographyCheckingResult(range:orthography:) 

Type Method

# orthographyCheckingResult(range:orthography:)

Creates and returns a text checking result with the specified orthography.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func orthographyCheckingResult(
    range: NSRange,
    orthography: NSOrthography
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`orthography`  

An orthography object that describes the script.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of orthography.

## See Also

### Text Checking Results for Orthography

var orthography: NSOrthography?

The detected orthography of a type checking result.

