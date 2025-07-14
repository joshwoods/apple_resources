

- Foundation
- NSPredicate
-  init(\_:) 

Initializer

# init(\_:)

Creates a predicate by converting an existing predicate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init?(_ predicate: Predicate) where Input : NSObject
```

## Parameters 

`predicate`  

The predicate to convert.

## Return Value

The converted predicate, or `nil` if conversion fails.

## Discussion

Only a subset of predicates that can be expressed by Predicate are convertible to NSPredicate. Predicates that include operations like the following can’t be converted:

- Accessing key paths for properties that aren’t exposed to the Objective-C runtime.

- Capturing values of types that aren’t supported by `NSPredicate`, like custom Swift structures.

- Using some functions or operators, like performing collection operations on a nonstring value.

## See Also

### Creating a Predicate

init(format: String, argumentArray: [Any]?)

Creates a predicate by substituting the values in a specified array into a format string and parsing the result.

init(format: String, arguments: CVaListPointer)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

convenience init(format: String, any CVarArg...)

Creates a predicate by substituting the values in an argument list into a format string and parsing the result.

func withSubstitutionVariables([String : Any]) -> Self

Returns a copy of the predicate and substitutes the predicates variables with specified values from a specified substitution variables dictionary.

init(value: Bool)

Creates and returns a predicate that always evaluates to a specified Boolean value.

init(block: (Any?, [String : Any]?) -> Bool)

Creates a predicate that evaluates using a specified block object and bindings dictionary.

init?(fromMetadataQueryString: String)

Creates a predicate with a metadata query string.

