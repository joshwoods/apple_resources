

- PassKit (Apple Pay and Wallet)
- PKContact
-  supplementarySubLocality Deprecated

Instance Property

# supplementarySubLocality

The contact’s sublocality, or `nil` if the sublocality is not needed for the transaction.

iOS 9.2–10.3DeprecatediPadOS 9.2–10.3DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12+visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.2Deprecated

``` source
var supplementarySubLocality: String? { get set }
```

Deprecated

Use subLocality and subAdministrativeArea on -postalAddress instead

## Discussion

If the transaction requires the contact’s address, and the region requires a sublocality, then the Apple Pay sheet automatically prompts the user to enter their sublocality. The contact’s sublocality information is stored in this property.

## See Also

### Contact information

var emailAddress: String?

The contact’s email address, or `nil` if the contact’s email is not needed for the transaction.

var name: PersonNameComponents?

The contact’s first and last name, or `nil` if the contact’s name is not needed for the transaction.

var phoneNumber: CNPhoneNumber?

The contact’s telephone number, or `nil` if the contact’s phone number is not needed for the transaction.

var postalAddress: CNPostalAddress?

The contact’s full postal address.

