

- PassKit (Apple Pay and Wallet)
-  PKContact 

Class

# PKContact

An object that encapsulates contact information needed for billing and shipping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
class PKContact
```

## Overview

Instances contain only the information needed for the given transaction. All other properties are set to `nil`.

## Topics

### Contact information

var emailAddress: String?

The contact’s email address, or `nil` if the contact’s email is not needed for the transaction.

var name: PersonNameComponents?

The contact’s first and last name, or `nil` if the contact’s name is not needed for the transaction.

var phoneNumber: CNPhoneNumber?

The contact’s telephone number, or `nil` if the contact’s phone number is not needed for the transaction.

var postalAddress: CNPostalAddress?

The contact’s full postal address.

var supplementarySubLocality: String?

The contact’s sublocality, or `nil` if the sublocality is not needed for the transaction.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with billing and shipping information

var billingContact: PKContact?

The user-selected billing address for this transaction.

var shippingContact: PKContact?

The user-selected shipping address for this transaction.

var shippingMethod: PKShippingMethod?

The user-selected shipping method for this transaction.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

