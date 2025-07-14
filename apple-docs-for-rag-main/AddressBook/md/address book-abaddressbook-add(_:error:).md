

- Address Book
- ABAddressBook
-  add(\_:error:) 

Instance Method

# add(\_:error:)

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

macOS 10.7+

``` source
func add(
    _ record: ABRecord!,
    error: ()
) throws
```

## Parameters 

`record`  

The record to add.

`error`  

A pointer to an error object that is set to an `NSError` instance if an error occurs.

## Discussion

If the `record` argument is `nil`, this method raises an exception. Your changes are not committed until you call the save() method.

It is more efficient to use the ABRecord method init(addressBook:) when possible.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Adding and Removing Records

func add(ABRecord!) -> Bool

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func remove(ABRecord!, error: ()) throws

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

func remove(ABRecord!) -> Bool

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

