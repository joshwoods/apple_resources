

- Contacts
- CNContact
-  identifier 

Instance Property

# identifier

A value that uniquely identifies a contact on the device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String { get }
```

## Discussion

It is recommended that you use the identifier when re-fetching the contact. An identifier can be persisted between the app launches. Note that this identifier only uniquely identifies the contact on the current device.

## See Also

### Identifying the Contact

var contactType: CNContactType

An enum identifying the contact type.

enum CNContactType

The types a contact can be.

