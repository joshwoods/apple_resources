

- Foundation
- NSPredicate
-  init(format:arguments:) 

Initializer

# init(format:arguments:)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format predicateFormat: String,
    arguments argList: CVaListPointer
)
```

## Parameters 

`predicateFormat`  

The format string for the new predicate.

`argList`  

The arguments to substitute into `predicateFormat`. Values are substituted in the order they appear in the argument list.

## Return Value

A new predicate by substituting the values in `argList` into `predicateFormat` and parsing the result.

## Discussion

For details of the format of the format string and of limitations on variable substitution, see Predicate Format String Syntax.

## See Also

### Creating a Predicate

init(format: String, argumentArray: [Any]?)

Creates a predicate by substituting the values in a specified array into a format string and parsing the result.

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

init?(fromMetadataQueryString: String)

Creates a predicate with a metadata query string.

