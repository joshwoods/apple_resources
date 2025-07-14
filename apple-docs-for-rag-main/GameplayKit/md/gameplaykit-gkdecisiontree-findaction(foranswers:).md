

- GameplayKit
- GKDecisionTree
-  findAction(forAnswers:) 

Instance Method

# findAction(forAnswers:)

Searches the decision tree, following the branches corresponding to each of the specified answers, and returns the resulting action object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func findAction(forAnswers answers: [AnyHashable : any NSObjectProtocol]) -> (any NSObjectProtocol)?
```

## Parameters 

`answers`  

A dictionary mapping attributes (or questions) to values (or answers to those questions).

## Return Value

The action object resulting from the decision-making process.

## Discussion

Actions can be any type of object relevant to your game; you define action objects when creating the tree. Typically, an action object is a string or simple value type identifying the result of the decision-making process in the context of your game.

In a manually created decision tree, an action is the “attribute” of a leaf node in the tree. That is, if you create a node using a method such as createBranch(value:attribute:), and create no further branches from that node, the `attribute` parameter of that node is treated as an action when evaluating the tree.

In an automatically learned decision tree, you provide action values with the init(examples:actions:attributes:) initializer.

Note

If a tree contains random branches (defined with the createBranch(weight:attribute:) method), you do not need to provide an answer for the corresponding attribute when finding an action.

## See Also

### Evaluating a Tree to Make Decisions

var randomSource: GKRandomSource

The randomizer to be used when evaluating parts of the tree that branch randomly.

