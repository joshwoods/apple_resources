

- Address Book
- ABAddressBook
-  remove(\_:error:) 

Instance Method

# remove(\_:error:)

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

macOS 10.7+

``` source
func remove(
    _ record: ABRecord!,
    error: ()
) throws
```

## Parameters 

`record`  

The record to be removed.

`error`  

A pointer to an error object that is set to an `NSError` instance if an error occurs.

## Discussion

If `record` is `nil`, this method raises an exception. Your changes are not committed until you call the save() method.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Adding and Removing Records

func add(ABRecord!, error: ()) throws

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func add(ABRecord!) -> Bool

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func remove(ABRecord!) -> Bool

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

