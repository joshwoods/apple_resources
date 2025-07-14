

- Open Directory
- ODNode
-  nodeName 

Instance Property

# nodeName

The node’s name.

Mac CatalystmacOS 10.6+

``` source
var nodeName: String! { get }
```

## See Also

### Querying a Node

func customCall(Int, send: Data!) throws -> Data

Returns the result of a custom call to the node.

func nodeDetails(forKeys: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary containing details about a node.

func subnodeNames() throws -> [Any]

Returns the names of subnodes for the node.

func unreachableSubnodeNames() throws -> [Any]

Returns an array of the subnodes of a given node that are currently unreachable.

