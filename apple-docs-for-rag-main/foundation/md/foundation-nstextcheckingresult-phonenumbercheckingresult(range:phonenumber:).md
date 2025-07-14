

- Foundation
- NSTextCheckingResult
-  phoneNumberCheckingResult(range:phoneNumber:) 

Type Method

# phoneNumberCheckingResult(range:phoneNumber:)

Creates and returns a text checking result with the specified phone number.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func phoneNumberCheckingResult(
    range: NSRange,
    phoneNumber: String
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`phoneNumber`  

The phone number.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of phoneNumber.

## See Also

### Text Checking Results for Phone Numbers

var phoneNumber: String?

The phone number of a type checking result.

