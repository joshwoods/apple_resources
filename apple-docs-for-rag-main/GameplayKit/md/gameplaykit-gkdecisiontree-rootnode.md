

- GameplayKit
- GKDecisionTree
-  rootNode 

Instance Property

# rootNode

The decision node at the root of the decision tree, representing the first attribute to test.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var rootNode: GKDecisionNode? { get }
```

## Discussion

To build a manually defined tree, use GKDecisionNode methods on that object to create branches leading to child nodes that represent additional attributes to test or final actions.

## See Also

### Creating a Manually Defined Decision Tree

init(attribute: any NSObjectProtocol)

Creates a decision tree starting with the specified initial attribute to test.

