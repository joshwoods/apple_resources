

- Foundation
- NSPredicate
-  init(format:\_:) 

Initializer

# init(format:\_:)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    format predicateFormat: String,
    _ args: any CVarArg...
)
```

## Parameters 

`predicateFormat`  

The format string for the new predicate.

`args`  

The arguments to substitute into `predicateFormat`.

## See Also

### Creating a Predicate

init(format: String, argumentArray: [Any]?)

Creates a predicate by substituting the values in a specified array into a format string and parsing the result.

init(format: String, arguments: CVaListPointer)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

convenience init?&lt;Input>(Predicate&lt;Input>)

Creates a predicate by converting an existing predicate.

func withSubstitutionVariables([String : Any]) -> Self

Returns a copy of the predicate and substitutes the predicates variables with specified values from a specified substitution variables dictionary.

init(value: Bool)

Creates and returns a predicate that always evaluates to a specified Boolean value.

init(block: (Any?, [String : Any]?) -> Bool)

Creates a predicate that evaluates using a specified block object and bindings dictionary.

init?(fromMetadataQueryString: String)

Creates a predicate with a metadata query string.

