

- PassKit (Apple Pay and Wallet)
- PKContact
-  emailAddress 

Instance Property

# emailAddress

The contact’s email address, or `nil` if the contact’s email is not needed for the transaction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
var emailAddress: String? { get set }
```

## See Also

### Contact information

var name: PersonNameComponents?

The contact’s first and last name, or `nil` if the contact’s name is not needed for the transaction.

var phoneNumber: CNPhoneNumber?

The contact’s telephone number, or `nil` if the contact’s phone number is not needed for the transaction.

var postalAddress: CNPostalAddress?

The contact’s full postal address.

var supplementarySubLocality: String?

The contact’s sublocality, or `nil` if the sublocality is not needed for the transaction.

Deprecated

