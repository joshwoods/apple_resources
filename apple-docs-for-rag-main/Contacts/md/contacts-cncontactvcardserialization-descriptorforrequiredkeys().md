

- Contacts
- CNContactVCardSerialization
-  descriptorForRequiredKeys() 

Type Method

# descriptorForRequiredKeys()

Use to fetch all contact keys required to create vCard data from a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func descriptorForRequiredKeys() -> any CNKeyDescriptor
```

## Return Value

A key descriptor to be used in the keysToFetch array when fetching the contacts.

