

- Foundation
- NSTextCheckingResult
-  phoneNumber 

Instance Property

# phoneNumber

The phone number of a type checking result.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var phoneNumber: String? { get }
```

## See Also

### Text Checking Results for Phone Numbers

class func phoneNumberCheckingResult(range: NSRange, phoneNumber: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified phone number.

