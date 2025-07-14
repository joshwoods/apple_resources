

- GameplayKit
-  GKDecisionTree 

Class

# GKDecisionTree

A data structure that models a set of specific questions, their possible answers, and the actions that follow from a series of answers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKDecisionTree
```

## Overview

You can define a decision tree manually, by specifying questions, answers, and actions, or you can allow the GKDecisionTree class to automatically learn a predictive model based on example data. A decision tree has several elements:

- *Attributes* represent individual questions to be answered or choices to be made.

- *Branches* are the possible answers to the questions or choices posed by each attribute.

- *Actions* are the final outcomes of the tree’s decision-making process. Each branch from an attribute leads either to another attribute or to an action.

When you use the GKDecisionTree class, attributes and actions can be any object type relevant to your app or game. You can define branches for specific answer values, using predicates, or with weights that influence a random decision. For example, a strategy combat game might use a decision tree to choose what a character should do on its turn, based on several criteria about the match in progress. In this case:

- For attributes, you might use (non-user-visible) strings that represent those criteria, such as `"Type?"` (what type of enemy is the character’s opponent?), `"HP?"` (how much health does the opponent have remaining?), and `"Special?"` (is the character’s special move available for use?).

- For branches, you’d use an appropriate style for each attribute. The `"Type?"` attribute might have a branch for each possible enemy type, but the `"HP?"` attribute could use predicates to determine whether the enemy’s health is above or below a certain threshold value.

- For actions, you might define your own enumerated type representing the kinds of attacks the character can choose (such as `Pound`, `Tackle`, and `Barrier`). Alternately, you might use instances of your own custom classes representing items or spells available to the character.

Figure 1 illustrates a possible tree structure based on the above example attributes, branches, and actions.

### Creating a Decision Tree

The GKDecisionTree class offers two ways to create decision trees.

In a *manually defined decision tree*, you define each attribute to be tested (or question to be asked), the possible branches (or answers) from each attribute, and the actions (or final outcomes) resulting from each complete series of attribute tests and branches. To manually create a tree, start by using the init(attribute:) initializer to define the first question to be asked. Then, use GKDecisionNode methods on the new tree’s rootNode object to define branches and the child nodes they lead to, with accompanying attribute or action values.

In a *learned decision tree*, you provide a set of attributes (or questions); a body of example items, each of which represents a set of attribute values (or answers to questions); and the final action to be taken for each example. The GKDecisionTree class then automatically infers a decision tree structure that, when presented with a set of attribute values matching or similar to one of your examples, predicts the corresponding action. To create a learned decision tree, use the init(examples:actions:attributes:) initializer. The following table shows sample input for a learned decision tree (based on the same hypothetical game shown in Figure 1).

| Opponent Type  (“Type?” attribute) | Opponent Health  (“HP?” attribute) | Can Use Special Move  (“Special?” attribute) | Move to Use  (Action) |
|----|----|----|----|
| Electric | 10 | Yes | Psychic Strike |
| Electric | 30 | No | Pound |
| Electric | 40 | Yes | Barrier |
| Fire | 10 | Yes | Pound |
| Fire | 30 | No | Tackle |
| Water | 10 | No | Pound |
| Water | 40 | No | Tackle |

After creating either kind of decision tree, you can use the inherited description property to examine its structure.

### Making Decisions

After you’ve created a tree, use the findAction(forAnswers:) method to evaluate it and choose an action. When you call that method, you provide a set of inputs (values for attributes, or answers to questions), and the tree follows the branches corresponding to each input value to produce an action.

Tip

When defining an attribute with a small set of possible values, define your own enum type to name the possible values. Then use the underlying numeric value of that enum when building trees with the GKDecisionNode createBranch(value:attribute:) method or the init(examples:actions:attributes:) initializer, and when passing a set of attribute values to the findAction(forAnswers:) method.

For example, the following code evaluates a tree similar to the examples in Figure 1 and the table above:

- Swift
- Objective-C

```
let answers = [
    "Type?": MyEnemyType.Electric.rawValue, // an enum value
    "HP?": 20,
    "Special?": true,
]
let action = myDecisionTree.findAction(forAnswers: answers)
```

```
NSDictionary *answers = @{
    @"Type?" : @(MyEnemyTypeElectric), // an enum value
    @"HP?" : @20,
    @"Special?" : @YES,
};
NSString *action = [myDecisionTree findActionForAnswers:answers];
```

## Topics

### Creating a Manually Defined Decision Tree

init(attribute: any NSObjectProtocol)

Creates a decision tree starting with the specified initial attribute to test.

var rootNode: GKDecisionNode?

The decision node at the root of the decision tree, representing the first attribute to test.

### Creating a Learned Decision Tree

init(examples: [[any NSObjectProtocol]], actions: [any NSObjectProtocol], attributes: [any NSObjectProtocol])

Creates an automatically learned decision tree using the specified attributes, example items, and actions.

### Evaluating a Tree to Make Decisions

func findAction(forAnswers: [AnyHashable : any NSObjectProtocol]) -> (any NSObjectProtocol)?

Searches the decision tree, following the branches corresponding to each of the specified answers, and returns the resulting action object.

var randomSource: GKRandomSource

The randomizer to be used when evaluating parts of the tree that branch randomly.

### Initializers

init(url: URL, error: (any Error)?)

### Instance Methods

func export(to: URL, error: (any Error)?) -> Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Decision Trees

class GKDecisionNode

A node for use in manually creating decision trees, representing a specific question and possible answers, or an action that follows from answering other questions.

