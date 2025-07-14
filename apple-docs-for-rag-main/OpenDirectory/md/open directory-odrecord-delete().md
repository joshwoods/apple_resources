

- Open Directory
- ODRecord
-  delete() 

Instance Method

# delete()

Deletes the record from its node and invalidates it.

Mac CatalystmacOS 10.6+

``` source
func delete() throws
```

## Discussion

The record should be released after this method is called.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

