

- Foundation
- NSPredicate
-  evaluate(with:substitutionVariables:) 

Instance Method

# evaluate(with:substitutionVariables:)

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies after substituting in the values from a specified variables dictionary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func evaluate(
    with object: Any?,
    substitutionVariables bindings: [String : Any]?
) -> Bool
```

## Parameters 

`object`  

The object against which to evaluate the predicate.

`bindings`  

The substitution variables dictionary. The dictionary must contain key-value pairs for all variables in the predicate.

## Return Value

true if `object` matches the conditions specified by the predicate after substituting in the values in `bindings` for any replacement tokens, otherwise false.

## Discussion

This method returns the same result as the two step process of first invoking withSubstitutionVariables(_:) on the predicate and then invoking evaluate(with:) on the returned value. This method is optimized for situations which require repeatedly evaluating a predicate with substitution variables with different variable substitutions.

## See Also

### Evaluating a Predicate

func evaluate(with: Any?) -> Bool

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies.

func allowEvaluation()

Forces a securely decoded predicate to allow evaluation.

