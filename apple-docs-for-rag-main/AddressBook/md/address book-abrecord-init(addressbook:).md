

- Address Book
- ABRecord
-  init(addressBook:) 

Initializer

# init(addressBook:)

Initializes a record using the given address book.

macOS 10.5+

``` source
init!(addressBook: ABAddressBook!)
```

## Parameters 

`addressBook`  

The address book with which to initialize the record.

## Discussion

The record is added to `addressBook` but is not visible to other address books until `addressBook` is saved. This method is the designated initializer for this class.

## See Also

### Creating a Record

init!()

Initializes a record using the shared address book.

