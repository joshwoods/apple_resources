

- Open Directory
- ODNode
-  init(session:type:) 

Initializer

# init(session:type:)

Creates a node object with a specified session and type.

Mac CatalystmacOS 10.6+

``` source
init(
    session inSession: ODSession!,
    type inType: ODNodeType
) throws
```

## Parameters 

`inSession`  

The session.

`inType`  

The node type.

## Return Value

The created node object.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating and Initializing a Node

init(session: ODSession!, name: String!) throws

Creates a node object with a specified session and name.

