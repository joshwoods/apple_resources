

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  disbursementCardUnsupportedError() 

Type Method

# disbursementCardUnsupportedError()

Creates an error that indicates that the selected payment pass doesn’t support receiving funds through disbursements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
class func disbursementCardUnsupportedError() -> any Error
```

## Return Value

An NSError that describes the error condition.

## See Also

### Handling errors

class func disbursementContactInvalidError(withContactField: PKContactField, localizedDescription: String?) -> any Error

Creates a recipient contact error with the supplied field.

