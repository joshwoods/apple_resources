

- Address Book
- ABAddressBook
-  saveAndReturnError() 

Instance Method

# saveAndReturnError()

Saves all the changes made since the last save.

macOS 10.5+

``` source
func saveAndReturnError() throws
```

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Saving and Detecting Changes

func hasUnsavedChanges() -> Bool

Indicates whether an address book has changes that have not been saved to the Address Book database.

func save() -> Bool

Saves all the changes made since the last save.

