

- Create ML
- MLWordTagger
- MLWordTagger.FeatureExtractorType
-  hashValue 

Instance Property

# hashValue

The hash value.

macOS 11.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Accessing the hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

