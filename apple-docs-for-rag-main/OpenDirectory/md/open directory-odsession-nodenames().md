

- Open Directory
- ODSession
-  nodeNames() 

Instance Method

# nodeNames()

Returns the node names that are registered with this session.

Mac CatalystmacOS 10.6+

``` source
func nodeNames() throws -> [Any]
```

## Return Value

The node names registered with this session.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

