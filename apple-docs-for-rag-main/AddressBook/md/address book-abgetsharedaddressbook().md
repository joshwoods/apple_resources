

- Address Book
-  ABGetSharedAddressBook() 

Function

# ABGetSharedAddressBook()

Returns the unique shared ABAddressBook object.

macOS

``` source
func ABGetSharedAddressBook() -> Unmanaged!
```

## Return Value

The address book for the logged-in user. You are responsible for retaining and releasing this object as needed.

## Discussion

Every application shares the address book for the logged-in user and this function returns it. If you call this function more than once or try to create a new address book, you get a pointer to the same shared address book.

## See Also

### Address Book

func ABCopyDefaultCountryCode(ABAddressBookRef!) -> Unmanaged&lt;CFString>!

Returns the default country code for records with unspecified country codes.

func ABHasUnsavedChanges(ABAddressBookRef!) -> Bool

Returns whether if there are unsaved changes in the address book.

func ABSave(ABAddressBookRef!) -> Bool

Saves all the changes made since the last save.

