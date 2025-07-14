

- Contacts
- CNContact
-  contactRelations 

Instance Property

# contactRelations

An array of labeled relations for the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var contactRelations: [CNLabeledValue] { get }
```

## Discussion

This property is an array of CNLabeledValue objects, each of which has a label and a CNContactRelation value. This property was previously known as related names.

## See Also

### Getting Related Information

var instantMessageAddresses: [CNLabeledValue&lt;CNInstantMessageAddress>]

An array of labeled IM addresses for the contact.

