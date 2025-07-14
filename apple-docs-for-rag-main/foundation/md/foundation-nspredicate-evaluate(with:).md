

- Foundation
- NSPredicate
-  evaluate(with:) 

Instance Method

# evaluate(with:)

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func evaluate(with object: Any?) -> Bool
```

## Parameters 

`object`  

The object against which to evaluate the predicate.

## Return Value

true if `object` matches the conditions specified by the predicate, otherwise false.

## See Also

### Evaluating a Predicate

func evaluate(with: Any?, substitutionVariables: [String : Any]?) -> Bool

Returns a Boolean value that indicates whether the specified object matches the conditions that the predicate specifies after substituting in the values from a specified variables dictionary.

func allowEvaluation()

Forces a securely decoded predicate to allow evaluation.

