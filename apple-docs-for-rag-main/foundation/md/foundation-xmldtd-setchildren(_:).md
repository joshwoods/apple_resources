

- Foundation
- XMLDTD
-  setChildren(\_:) 

Instance Method

# setChildren(\_:)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setChildren(_ children: [XMLNode]?)
```

## Parameters 

`children`  

An array of XMLNode objects. To remove all existing children, pass in `nil`.

## Discussion

Replaced or removed child nodes are released.

## See Also

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

