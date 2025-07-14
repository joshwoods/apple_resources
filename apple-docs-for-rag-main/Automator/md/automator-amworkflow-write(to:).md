

- Automator
- AMWorkflow
-  write(to:) 

Instance Method

# write(to:)

Writes the workflow to the specified file.

Mac Catalyst 14.0+macOS 10.4+

``` source
func write(to fileURL: URL) throws
```

## Parameters 

`fileURL`  

URL that specifies the file location to write the workflow.

## Discussion

You might want to save the workflow, for example, because you have made changes to a variable it contains.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

