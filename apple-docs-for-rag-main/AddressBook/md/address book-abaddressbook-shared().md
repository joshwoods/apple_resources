

- Address Book
- ABAddressBook
-  shared() 

Type Method

# shared()

Returns the unique shared instance of `ABAddressBook`, or `nil` if the Address Book database can’t be initialized.

macOS

``` source
class func shared() -> ABAddressBook!
```

## Return Value

The unique shared instance of `ABAddressBook`, or `nil` if the Address Book database can’t be initialized.

## Discussion

This method returns the address book for the logged-in user that is shared by every application. If you call this method more than once or try to create a new address book, you will get a pointer to the same shared address book.

If you’re just making one-off lookups and edits, this is the appropriate method to use. If your code is executing a tight loop, using the addressBook method with the init(addressBook:) method of ABPerson can yield significant performance improvements. See Accessing the Address Book for more details.

If the user denies your application access to the Address Book database, this method returns `nil`.

