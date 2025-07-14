

- Core Spotlight
- CSCustomAttributeKey
-  init(keyName:searchable:searchableByDefault:unique:multiValued:) 

Initializer

# init(keyName:searchable:searchableByDefault:unique:multiValued:)

Returns a new custom attribute key with the specified name and properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init?(
    keyName: String,
    searchable: Bool,
    searchableByDefault: Bool,
    unique: Bool,
    multiValued: Bool
)
```

## Parameters 

`keyName`  

The name of the custom attribute for use as a key in a CSSearchableItemAttributeSet. The key name must be a string that contains only ASCII characters and no punctuation other than the underscore (that is, “\_”). The prefix `kMD` is reserved.

`searchable`  

A Boolean value that indicates if the attribute can be specified as a search term.

`searchableByDefault`  

A Boolean value that indicates if the attribute should be searchable by default.

`unique`  

A Boolean value that indicates if duplicate values should be treated as the same value to save storage space.

`multiValued`  

A Boolean value that indicates if the attribute is likely to have multiple values, such as arrays, associated with it.

## Return Value

A new custom attribute key with the specified name and properties.

## Discussion

To create custom attribute key names, it’s recommended that you use a reverse DNS format that includes your company name and does not include the period character (”.”). For example, a key name of the form `com_mycompany_myapp_mykeyname` works well.

## See Also

### Creating a custom attribute

convenience init?(keyName: String)

Returns a new custom attribute key with the specified name.

