

- MusicKit
- MusicCatalogChart
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var hashValue: Int { get }
```

Available when `MusicItemType` conforms to `MusicCatalogChartRequestable` and `Hashable`.

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

