

- Foundation
- NSTextCheckingResult
-  addressComponents 

Instance Property

# addressComponents

The address dictionary of a type checking result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var addressComponents: [NSTextCheckingKey : String]? { get }
```

## Discussion

The dictionary keys are described in Keys for Address Components.

## See Also

### Text Checking Results for Addresses

class func addressCheckingResult(range: NSRange, components: [NSTextCheckingKey : String]) -> NSTextCheckingResult

Creates and returns a text checking result with the specified address components.

