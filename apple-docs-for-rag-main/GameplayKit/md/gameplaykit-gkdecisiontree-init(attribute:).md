

- GameplayKit
- GKDecisionTree
-  init(attribute:) 

Initializer

# init(attribute:)

Creates a decision tree starting with the specified initial attribute to test.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(attribute: any NSObjectProtocol)
```

## Parameters 

`attribute`  

The first attribute to test (or question to answer) when evaluating the tree.

## Return Value

A new decision tree.

## Discussion

The decision tree returned by this initializer is incomplete. To build a manually defined tree, use the rootNode property to access the node corresponding to the initial attribute, and use GKDecisionNode methods on that object to create branches leading to child nodes that represent additional attributes to test or final actions.

## See Also

### Creating a Manually Defined Decision Tree

var rootNode: GKDecisionNode?

The decision node at the root of the decision tree, representing the first attribute to test.

