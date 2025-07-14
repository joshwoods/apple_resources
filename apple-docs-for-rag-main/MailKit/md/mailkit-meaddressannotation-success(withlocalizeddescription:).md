

- MailKit
- MEAddressAnnotation
-  success(withLocalizedDescription:) 

Type Method

# success(withLocalizedDescription:)

Indicates an address is valid and correct.

macOS 12.0+

``` source
class func success(withLocalizedDescription localizedDescription: String) -> MEAddressAnnotation
```

## Parameters 

`localizedDescription`  

A user-visible string with details about the address, such as the full name of the recipient.

## Return Value

An annotation that indicates an email address is valid.

## See Also

### Specifying Email Address Validity

class func warning(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address may be invalid or needs attention.

class func error(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is invalid and may result in failure to deliver a message.

