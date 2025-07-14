

- PackageDescription
- LanguageTag
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the language tag by feeding the item into the given hasher.

PackageDescriptionSwift

``` source
func hash(into hasher: inout Hasher)
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Hashing

var hashValue: Int

The hash value for language tag.

