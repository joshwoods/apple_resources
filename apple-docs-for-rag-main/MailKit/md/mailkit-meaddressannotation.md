

- MailKit
-  MEAddressAnnotation 

Class

# MEAddressAnnotation

An object that indicates the validity of an email address.

macOS 12.0+

``` source
class MEAddressAnnotation
```

## Overview

Mail displays the status of an annotation as part of the address tokens in the To, Cc, and Bcc fields using a status icon and color.

## Topics

### Specifying Email Address Validity

class func success(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is valid and correct.

class func warning(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address may be invalid or needs attention.

class func error(withLocalizedDescription: String) -> MEAddressAnnotation

Indicates an address is invalid and may result in failure to deliver a message.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Annotating Email Address Tokens

func annotateAddressesForSession(MEComposeSession, completion: ([MEEmailAddress : MEAddressAnnotation]) -> Void)

Indicates whether recipients in the compose window are valid or not.

