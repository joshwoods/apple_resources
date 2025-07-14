

- GameplayKit
- GKDecisionTree
-  randomSource 

Instance Property

# randomSource

The randomizer to be used when evaluating parts of the tree that branch randomly.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
@NSCopying
var randomSource: GKRandomSource { get set }
```

## Discussion

Some of the branches in a decision tree may not depend on an external input; instead, when evaluating the tree with the findAction(forAnswers:) method, the tree automatically chooses an answer at random. (In a manually created decision tree, you can create random branches with the createBranch(weight:attribute:) method.) The tree uses this random source when randomly choosing answers.

## See Also

### Evaluating a Tree to Make Decisions

func findAction(forAnswers: [AnyHashable : any NSObjectProtocol]) -> (any NSObjectProtocol)?

Searches the decision tree, following the branches corresponding to each of the specified answers, and returns the resulting action object.

