

- Foundation
- NSPredicate
-  withSubstitutionVariables(\_:) 

Instance Method

# withSubstitutionVariables(\_:)

Returns a copy of the predicate and substitutes the predicates variables with specified values from a specified substitution variables dictionary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withSubstitutionVariables(_ variables: [String : Any]) -> Self
```

## Parameters 

`variables`  

The substitution variables dictionary. The dictionary must contain key-value pairs for all variables in the receiver.

## Return Value

A copy of the receiver with the predicate’s variables substituted by values specified in `variables`.

## Discussion

The predicate itself is not modified by this method, so you can reuse it for any number of substitutions.

## See Also

### Creating a Predicate

init(format: String, argumentArray: [Any]?)

Creates a predicate by substituting the values in a specified array into a format string and parsing the result.

init(format: String, arguments: CVaListPointer)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

convenience init(format: String, any CVarArg...)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

convenience init?&lt;Input>(Predicate&lt;Input>)

Creates a predicate by converting an existing predicate.

init(value: Bool)

Creates and returns a predicate that always evaluates to a specified Boolean value.

init(block: (Any?, [String : Any]?) -> Bool)

Creates a predicate that evaluates using a specified block object and bindings dictionary.

init?(fromMetadataQueryString: String)

Creates a predicate with a metadata query string.

