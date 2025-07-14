

- Foundation
- NSTextCheckingResult
-  transitInformationCheckingResult(range:components:) 

Type Method

# transitInformationCheckingResult(range:components:)

Creates and returns a text checking result with the specified transit information.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func transitInformationCheckingResult(
    range: NSRange,
    components: [NSTextCheckingKey : String]
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`components`  

A dictionary containing the transit components. The currently supported keys are airline and flight.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of transitInformation.

