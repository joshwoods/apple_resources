

- Address Book UI
- ABNewPersonViewController
-  addressBook Deprecated

Instance Property

# addressBook

Optional. The address book to which the new contact is added.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var addressBook: ABAddressBook? { get set }
```

Deprecated

Use contactStore instead.

## Discussion

When unset, an address book is created and assigned to this property when needed.

## See Also

### Configuring New Person Views

var parentGroup: ABRecord?

Optional. Specifies the group to which to add the new contact on save.

Deprecated

