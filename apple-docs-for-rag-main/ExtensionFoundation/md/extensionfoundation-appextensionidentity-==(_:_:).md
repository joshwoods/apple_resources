

- ExtensionFoundation
- AppExtensionIdentity
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two extensions are equal

macOS 13.0+

``` source
static func == (lhs: AppExtensionIdentity, rhs: AppExtensionIdentity) -> Bool
```

## Parameters 

`lhs`  

The first extension to compare.

`rhs`  

The second extension to compare.

## Return Value

A Boolean value set to true if the two extension parameters are equal.

## See Also

### Comparing Extensions

func hash(into: inout Hasher)

Hashes the essential components of the extension by feeding them into the given hash function.

