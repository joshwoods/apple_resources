

- GameplayKit
- GKRuleSystem
-  minimumGrade(forFacts:) 

Instance Method

# minimumGrade(forFacts:)

Returns the lowest membership grade among the specified facts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func minimumGrade(forFacts facts: [Any]) -> Float
```

## Parameters 

`facts`  

An array of objects representing truths claimed or rejected by the rule system. For details, see the facts property.

## Return Value

The lowest membership grade in the array of facts.

## Discussion

In fuzzy logic, this method is called the AND Zadeh operator, because it corresponds to the AND operator in Boolean logic.

Note

If a fact is not in the facts array, its membership grade for purposes of this operation is implicitly zero.

## See Also

### Related Documentation

var facts: [Any]

The list of facts claimed by the rule system.

### Drawing Conclusions from Facts

func grade(forFact: any NSObjectProtocol) -> Float

Returns the membership grade of the specified fact.

func maximumGrade(forFacts: [Any]) -> Float

Returns the highest membership grade among the specified facts.

