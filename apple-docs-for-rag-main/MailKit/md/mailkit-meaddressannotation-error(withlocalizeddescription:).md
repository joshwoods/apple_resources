

- MailKit
- MEAddressAnnotation
-  error(withLocalizedDescription:) 

Type Method

# error(withLocalizedDescription:)

Indicates an address is invalid and may result in failure to deliver a message.

macOS 12.0+

``` source
class func error(withLocalizedDescription localizedDescription: String) -> MEAddressAnnotation
```

## Parameters 

`localizedDescription`  

A user-visible string with details about the reason the address is invalid.

## Return Value

An annotation that indicates an email address is invalid and may result in failure to deliver a message.

## See Also

### Specifying Email Address Validity

class func success(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is valid and correct.

class func warning(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address may be invalid or needs attention.

