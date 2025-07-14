

- Contacts
- CNMutableContact
-  postalAddresses 

Instance Property

# postalAddresses

An array of labeled postal addresses for a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var postalAddresses: [CNLabeledValue] { get set }
```

## Discussion

This property is an array of CNLabeledValue objects, each of which has a label and a CNPostalAddress value.

## See Also

### Setting Addresses

var emailAddresses: [CNLabeledValue&lt;NSString>]

An array of labeled email addresses for the contact.

var urlAddresses: [CNLabeledValue&lt;NSString>]

An array of labeled URL addresses for a contact.

