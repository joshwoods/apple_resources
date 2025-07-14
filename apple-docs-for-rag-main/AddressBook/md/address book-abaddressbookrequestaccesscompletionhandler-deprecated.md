

- Address Book
-  ABAddressBookRequestAccessCompletionHandler Deprecated

Type Alias

# ABAddressBookRequestAccessCompletionHandler

Definition for a block callback invoked when an access request has completed.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
typealias ABAddressBookRequestAccessCompletionHandler = (Bool, CFError?) -> Void
```

## Discussion

Address book request access completion handler blocks are used with ABAddressBookCreateWithOptions(_:_:). If you had a view controller that wanted to display the count of users with the name “Smith” in the address book, you might implement something like the code shown in the following code listing.

Listing 1. Sample implementation using ABAddressBookRequestAccessCompletionHandler

```
```

## See Also

### Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

typealias ABExternalChangeCallback

Prototype for a function callback invoked on an address book when the Address Book database is modified by another address book instance.

Deprecated

typealias ABMultiValueIdentifier

Identifies multivalue properties.

Deprecated

typealias ABPersonCompositeNameFormat

Indicates a person-name display format.

Deprecated

typealias ABPersonSortOrdering

Indicates a person sort ordering.

Deprecated

typealias ABPropertyID

Integer that identifies a record property.

Deprecated

typealias ABRecordID

Integer that identifies a record.

Deprecated

typealias ABRecordType

Integer that identifies a record type.

Deprecated

typealias ABSourceType

Indicates a source type. See `Source Properties`.

Deprecated

