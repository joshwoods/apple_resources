

- Foundation
- NSPredicate
-  init(block:) 

Initializer

# init(block:)

Creates a predicate that evaluates using a specified block object and bindings dictionary.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(block: @escaping (Any?, [String : Any]?) -> Bool)
```

## Parameters 

`block`  

The block is applied to the object to be evaluated.

The block takes two arguments:

evaluatedObject  
The object to be evaluated.

bindings  
The substitution variables dictionary. The dictionary must contain key-value pairs for all variables in the receiver.

The block returns true if the `evaluatedObject` evaluates to true, otherwise false.

## Return Value

A new predicate by that evaluates objects using `block`.

## Discussion

In macOS 10.6 and later, Core Data supports block-based predicates in the in-memory and atomic stores, but not in the SQLite-based store.

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

func withSubstitutionVariables([String : Any]) -> Self

Returns a copy of the predicate and substitutes the predicates variables with specified values from a specified substitution variables dictionary.

init(value: Bool)

Creates and returns a predicate that always evaluates to a specified Boolean value.

init?(fromMetadataQueryString: String)

Creates a predicate with a metadata query string.

