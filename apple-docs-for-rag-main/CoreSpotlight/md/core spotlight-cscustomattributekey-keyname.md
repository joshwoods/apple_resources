

- Core Spotlight
- CSCustomAttributeKey
-  keyName 

Instance Property

# keyName

The name of the custom attribute key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var keyName: String { get }
```

## Discussion

The key name is a string that contains only ASCII characters and no punctuation other than the underscore (that is “\_”). The prefix `kMD` is reserved. To create a custom attribute key name, it’s recommended that you use a reverse DNS format that includes your company name and does not include the period character (”.”). For example, a key name of the form `com_mycompany_myapp_mykeyname` works well.

## See Also

### Getting the attribute details

var isMultiValued: Bool

A Boolean value that indicates if the custom attribute is likely to have multiple values, such as arrays, associated with it.

var isSearchable: Bool

A Boolean value that indicates if the custom attribute can be specified as a search term.

var isSearchableByDefault: Bool

A Boolean value that indicates if the custom attribute should be searchable by default.

var isUnique: Bool

A Boolean value that indicates if duplicate custom attribute values should be treated as the same value to save storage space.

