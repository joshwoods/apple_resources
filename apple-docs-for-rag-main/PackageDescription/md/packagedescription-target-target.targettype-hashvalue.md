

- PackageDescription
- Target
- Target.TargetType
-  hashValue 

Instance Property

# hashValue

The target type’s hash value.

PackageDescriptionSwift

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Hashing

func hash(into: inout Hasher)

Hashes the target type by feeding the item into the given hasher.

