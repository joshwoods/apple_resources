

- Contacts
- CNContact
-  instantMessageAddresses 

Instance Property

# instantMessageAddresses

An array of labeled IM addresses for the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var instantMessageAddresses: [CNLabeledValue] { get }
```

## Discussion

This property is an array of CNLabeledValue objects, each of which has a label and a CNInstantMessageAddress value.

## See Also

### Getting Related Information

var contactRelations: [CNLabeledValue&lt;CNContactRelation>]

An array of labeled relations for the contact.

