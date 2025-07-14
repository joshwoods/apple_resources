

- Foundation
- NSTextCheckingResult
-  addressCheckingResult(range:components:) 

Type Method

# addressCheckingResult(range:components:)

Creates and returns a text checking result with the specified address components.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func addressCheckingResult(
    range: NSRange,
    components: [NSTextCheckingKey : String]
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`components`  

A dictionary containing the address components. The dictionary keys are described in Keys for Address Components.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of address.

## See Also

### Text Checking Results for Addresses

var addressComponents: [NSTextCheckingKey : String]?

The address dictionary of a type checking result.

