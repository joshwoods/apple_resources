

- Core Spotlight
- CSCustomAttributeKey
-  isMultiValued 

Instance Property

# isMultiValued

A Boolean value that indicates if the custom attribute is likely to have multiple values, such as arrays, associated with it.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var isMultiValued: Bool { get }
```

## Discussion

The default value of this property is `false`.

## See Also

### Getting the attribute details

var keyName: String

The name of the custom attribute key.

var isSearchable: Bool

A Boolean value that indicates if the custom attribute can be specified as a search term.

var isSearchableByDefault: Bool

A Boolean value that indicates if the custom attribute should be searchable by default.

var isUnique: Bool

A Boolean value that indicates if duplicate custom attribute values should be treated as the same value to save storage space.

