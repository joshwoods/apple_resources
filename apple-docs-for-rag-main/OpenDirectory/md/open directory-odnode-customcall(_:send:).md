

- Open Directory
- ODNode
-  customCall(\_:send:) 

Instance Method

# customCall(\_:send:)

Returns the result of a custom call to the node.

Mac CatalystmacOS 10.6+

``` source
func customCall(
    _ inCustomCode: Int,
    send inSendData: Data!
) throws -> Data
```

## Parameters 

`inCustomCode`  

The custom code to send to the node.

`inSendData`  

Data required by `inCustomCode`. Can be `nil`.

## Return Value

The result of the custom call.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Querying a Node

func nodeDetails(forKeys: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary containing details about a node.

var nodeName: String!

The node’s name.

func subnodeNames() throws -> [Any]

Returns the names of subnodes for the node.

func unreachableSubnodeNames() throws -> [Any]

Returns an array of the subnodes of a given node that are currently unreachable.

