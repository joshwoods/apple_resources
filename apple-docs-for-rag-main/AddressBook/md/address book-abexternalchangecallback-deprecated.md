

- Address Book
-  ABExternalChangeCallback Deprecated

Type Alias

# ABExternalChangeCallback

Prototype for a function callback invoked on an address book when the Address Book database is modified by another address book instance.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
typealias ABExternalChangeCallback = (ABAddressBook?, CFDictionary?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`addressBook`  

An address book used to interact with the Address Book database.

`info`  

Always `NULL`.

`context`  

The object to pass to the callback function.

## Discussion

If you name your callback function `MyAddressBookExternalChangeCallback`, you declare it like this:

### Discussion

Use ABAddressBookRegisterExternalChangeCallback(_:_:_:) to register and ABAddressBookUnregisterExternalChangeCallback(_:_:_:) to unregister the callback function.

You can register for a callback with different contexts or callback functions. The run loop on the thread that registered the callback invokes the callback.

The `addressBook` object does not take any action to flush or synchronize cached state with the Address Book database. If you want to ensure that `addressBook` doesn’t contain stale values, use ABAddressBookRevert(_:).

## See Also

### Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

typealias ABAddressBookRequestAccessCompletionHandler

Definition for a block callback invoked when an access request has completed.

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

