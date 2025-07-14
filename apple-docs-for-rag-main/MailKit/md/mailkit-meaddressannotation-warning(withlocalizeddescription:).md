

- MailKit
- MEAddressAnnotation
-  warning(withLocalizedDescription:) 

Type Method

# warning(withLocalizedDescription:)

Indicates an address may be invalid or needs attention.

macOS 12.0+

``` source
class func warning(withLocalizedDescription localizedDescription: String) -> MEAddressAnnotation
```

## Parameters 

`localizedDescription`  

A user-visible string with details about why the recipient needs attention.

## Return Value

An annotation that indicates an email address may not be valid or needs attention.

## See Also

### Specifying Email Address Validity

class func success(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is valid and correct.

class func error(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is invalid and may result in failure to deliver a message.

