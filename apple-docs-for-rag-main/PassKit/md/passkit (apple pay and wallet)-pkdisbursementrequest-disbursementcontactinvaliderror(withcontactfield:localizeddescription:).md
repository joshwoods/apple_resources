

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  disbursementContactInvalidError(withContactField:localizedDescription:) 

Type Method

# disbursementContactInvalidError(withContactField:localizedDescription:)

Creates a recipient contact error with the supplied field.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
class func disbursementContactInvalidError(
    withContactField field: PKContactField,
    localizedDescription: String?
) -> any Error
```

## Parameters 

`field`  

The PKContactField that contains the error.

`localizedDescription`  

An optional localized description that the framework displays to the individual.

## Return Value

An NSError object.

## Discussion

There’s limited display space available for descriptions, so keep your messages concise.

## See Also

### Handling errors

class func disbursementCardUnsupportedError() -> any Error

Creates an error that indicates that the selected payment pass doesn’t support receiving funds through disbursements.

