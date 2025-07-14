

- Address Book
- ABAddressBook
-  save() 

Instance Method

# save()

Saves all the changes made since the last save.

macOS

``` source
func save() -> Bool
```

## Return Value

true if successful or there were no changes; otherwise, false.

## See Also

### Saving and Detecting Changes

func hasUnsavedChanges() -> Bool

Indicates whether an address book has changes that have not been saved to the Address Book database.

func saveAndReturnError() throws

Saves all the changes made since the last save.

