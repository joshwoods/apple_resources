

- Open Directory
- ODNode
-  subnodeNames() 

Instance Method

# subnodeNames()

Returns the names of subnodes for the node.

Mac CatalystmacOS 10.6+

``` source
func subnodeNames() throws -> [Any]
```

## Return Value

An array of subnode names.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Querying a Node

func customCall(Int, send: Data!) throws -> Data

Returns the result of a custom call to the node.

func nodeDetails(forKeys: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary containing details about a node.

var nodeName: String!

The node’s name.

func unreachableSubnodeNames() throws -> [Any]

Returns an array of the subnodes of a given node that are currently unreachable.

