

- Foundation
- NSPredicate
-  init(fromMetadataQueryString:) 

Initializer

# init(fromMetadataQueryString:)

Creates a predicate with a metadata query string.

macOS 10.9+

``` source
init?(fromMetadataQueryString queryString: String)
```

## Parameters 

`queryString`  

A metadata query string.

## Discussion

For details of the format of the query string, see File Metadata Query Expression Syntax.

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

init(block: (Any?, [String : Any]?) -> Bool)

Creates a predicate that evaluates using a specified block object and bindings dictionary.

