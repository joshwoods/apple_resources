

- Foundation
- NSPredicate
-  allowEvaluation() 

Instance Method

# allowEvaluation()

Forces a securely decoded predicate to allow evaluation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func allowEvaluation()
```

## Discussion

When securely decoding NSPredicate objects that are encoded using NSSecureCoding, evaluation is disabled because it is potentially unsafe to evaluate predicates you get out of an archive.

Before you enable evaluation, you should validate key paths, selectors, and other details to ensure no erroneous or malicious code will be executed. Once you’ve verified the predicate, you can enable the receiver for evaluation by calling allowEvaluation().

## See Also

### Evaluating a Predicate

func evaluate(with: Any?) -> Bool

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies.

func evaluate(with: Any?, substitutionVariables: [String : Any]?) -> Bool

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies after substituting in the values from a specified variables dictionary.

