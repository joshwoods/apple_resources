

- Address Book
-  ABHasUnsavedChanges(\_:) 

Function

# ABHasUnsavedChanges(\_:)

Returns whether if there are unsaved changes in the address book.

macOS

``` source
func ABHasUnsavedChanges(_ addressBook: ABAddressBookRef!) -> Bool
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

## Return Value

`true` if there are unsaved changes, `false` otherwise.

## Discussion

The unsaved changes flag is set automatically whenever changes are made to the address book.

## See Also

### Address Book

func ABGetSharedAddressBook() -> Unmanaged&lt;ABAddressBookRef>!

Returns the unique shared ABAddressBook object.

func ABCopyDefaultCountryCode(ABAddressBookRef!) -> Unmanaged&lt;CFString>!

Returns the default country code for records with unspecified country codes.

func ABSave(ABAddressBookRef!) -> Bool

Saves all the changes made since the last save.

