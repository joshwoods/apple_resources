

- ExtensionFoundation
- AppExtensionIdentity
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the extension by feeding them into the given hash function.

macOS 13.0+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hash function to use when combining the components of the color parameter.

## See Also

### Comparing Extensions

static func == (AppExtensionIdentity, AppExtensionIdentity) -> Bool

Indicates whether two extensions are equal

