

- PassKit (Apple Pay and Wallet)
- PKContact
-  postalAddress 

Instance Property

# postalAddress

The contact’s full postal address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
var postalAddress: CNPostalAddress? { get set }
```

## Discussion

The contact’s full street address including name, street, city, state or province, postal code, and country or region. This property can be `nil` if the contact’s address isn’t needed for the transaction.

## See Also

### Contact information

var emailAddress: String?

The contact’s email address, or `nil` if the contact’s email is not needed for the transaction.

var name: PersonNameComponents?

The contact’s first and last name, or `nil` if the contact’s name is not needed for the transaction.

var phoneNumber: CNPhoneNumber?

The contact’s telephone number, or `nil` if the contact’s phone number is not needed for the transaction.

var supplementarySubLocality: String?

The contact’s sublocality, or `nil` if the sublocality is not needed for the transaction.

Deprecated

