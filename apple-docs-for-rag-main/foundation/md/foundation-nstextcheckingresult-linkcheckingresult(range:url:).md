

- Foundation
- NSTextCheckingResult
-  linkCheckingResult(range:url:) 

Type Method

# linkCheckingResult(range:url:)

Creates and returns a text checking result with the specified URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func linkCheckingResult(
    range: NSRange,
    url: URL
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`url`  

The URL.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of link.

## See Also

### Text Checking Results for URLs

var url: URL?

The URL of a type checking result.

