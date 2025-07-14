

- Address Book
- ABAddressBook
-  hasUnsavedChanges() 

Instance Method

# hasUnsavedChanges()

Indicates whether an address book has changes that have not been saved to the Address Book database.

macOS

``` source
func hasUnsavedChanges() -> Bool
```

## Return Value

`true` if there are unsaved changes; otherwise, `false`.

## Discussion

The unsaved changes flag is set automatically whenever changes are made.

## See Also

### Saving and Detecting Changes

func save() -> Bool

Saves all the changes made since the last save.

func saveAndReturnError() throws

Saves all the changes made since the last save.

