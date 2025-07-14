

- Address Book
-  ABCopyDefaultCountryCode(\_:) 

Function

# ABCopyDefaultCountryCode(\_:)

Returns the default country code for records with unspecified country codes.

macOS 10.3+

``` source
func ABCopyDefaultCountryCode(_ addressBook: ABAddressBookRef!) -> Unmanaged!
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

## Return Value

A string with the default country code. You are responsible for releasing this object.

## See Also

### Address Book

func ABGetSharedAddressBook() -> Unmanaged&lt;ABAddressBookRef>!

Returns the unique shared ABAddressBook object.

func ABHasUnsavedChanges(ABAddressBookRef!) -> Bool

Returns whether if there are unsaved changes in the address book.

func ABSave(ABAddressBookRef!) -> Bool

Saves all the changes made since the last save.

