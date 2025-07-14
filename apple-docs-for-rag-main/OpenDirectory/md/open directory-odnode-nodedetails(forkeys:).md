

- Open Directory
- ODNode
-  nodeDetails(forKeys:) 

Instance Method

# nodeDetails(forKeys:)

Returns a dictionary containing details about a node.

Mac CatalystmacOS 10.6+

``` source
func nodeDetails(forKeys inKeys: [Any]!) throws -> [AnyHashable : Any]
```

## Parameters 

`inKeys`  

An array of keys corresponding to the values returned in the dictionary.

## Return Value

A dictionary containing details about the node corresponding to keys specified by `inKeys`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Querying a Node

func customCall(Int, send: Data!) throws -> Data

Returns the result of a custom call to the node.

var nodeName: String!

The node’s name.

func subnodeNames() throws -> [Any]

Returns the names of subnodes for the node.

func unreachableSubnodeNames() throws -> [Any]

Returns an array of the subnodes of a given node that are currently unreachable.

