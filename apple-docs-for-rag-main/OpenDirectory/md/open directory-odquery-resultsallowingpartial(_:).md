

- Open Directory
- ODQuery
-  resultsAllowingPartial(\_:) 

Instance Method

# resultsAllowingPartial(\_:)

Returns results from a query synchronously.

Mac CatalystmacOS 10.6+

``` source
func resultsAllowingPartial(_ inAllowPartialResults: Bool) throws -> [Any]
```

## Parameters 

`inAllowPartialResults`  

If true, only immediately available results are returned; otherwise, the function waits until all results are available.

## Return Value

The results of the query in an array of `ODRecord` objects.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

