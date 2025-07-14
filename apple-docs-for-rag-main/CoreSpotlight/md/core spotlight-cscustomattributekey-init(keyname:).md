

- Core Spotlight
- CSCustomAttributeKey
-  init(keyName:) 

Initializer

# init(keyName:)

Returns a new custom attribute key with the specified name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
convenience init?(keyName: String)
```

## Parameters 

`keyName`  

The name of the custom attribute for use as a key in a CSSearchableItemAttributeSet. The key name must be a string that contains only ASCII characters and no punctuation other than the underscore (that is “\_”). The prefix `kMD` is reserved.

## Return Value

A new custom attribute key.

## Discussion

To create custom attribute key names, it’s recommended that you use a reverse DNS format that includes your company name and does not include the period character (”.”). For example, a key name of the form `com_mycompany_myapp_mykeyname` works well.

## See Also

### Creating a custom attribute

init?(keyName: String, searchable: Bool, searchableByDefault: Bool, unique: Bool, multiValued: Bool)

Returns a new custom attribute key with the specified name and properties.

