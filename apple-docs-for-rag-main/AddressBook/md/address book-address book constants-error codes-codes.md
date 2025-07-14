

- Address Book
- Address Book Constants
-  Error Codes 

API Collection

# Error Codes

Errors codes used by the Address Book framework.

## Topics

### Errors

var ABAddRecordsError: Int

The records could not be added.

var ABRemoveRecordsError: Int

The records could not be removed.

var ABPropertyValueValidationError: Int

The property value is not valid.

var ABPropertyUnsupportedBySourceError: Int

The property is not supported by the source.

var ABPropertyReadOnlyError: Int

The property is read-only.

### Dictionary Keys

let ABMultiValueIdentifiersErrorKey: String

Key used with ABPropertyValueValidationError.

## See Also

### Errors

let ABAddressBookErrorDomain: CFString!

Error domain returning errors reported by an address book object.

Deprecated

