

- Automator
- AMWorkflow
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates and initializes a workflow based on the contents of the specified file.

Mac Catalyst 14.0+macOS 10.4+

``` source
convenience init(contentsOf fileURL: URL) throws
```

## Parameters 

`fileURL`  

URL that specifies the location of a workflow file.

## Return Value

The initialized workflow object. On error, returns nil.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating a Workflow

init()

Creates and initializes a workflow.

