

- Foundation
- CodableConfiguration
-  init(wrappedValue:from:) 

Initializer

# init(wrappedValue:from:)

Creates a codable configuration wrapper for the given value, using given configuration provider type identified by key path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    wrappedValue: T,
    from keyPath: KeyPath
)
```

Available when `T` conforms to `DecodableWithConfiguration`, `T` conforms to `EncodableWithConfiguration`, `ConfigurationProvider` conforms to `AttributeScope`, `T.DecodingConfiguration` is `ConfigurationProvider.DecodingConfiguration`, and `T.EncodingConfiguration` is `ConfigurationProvider.EncodingConfiguration`.

## Parameters 

`wrappedValue`  

The underlying value to make codable, using data from the configuration provider.

`keyPath`  

A key path that identifies the type of the configuration provider, which provides additional information to encode `wrappedValue`.

## See Also

### Creating a Codable Configuration

init(wrappedValue: T)

Creates a codable configuration wrapper for the given value.

init(wrappedValue: T, from: ConfigurationProvider.Type)

Creates a codable configuration wrapper for the given value, using the given configuration provider type.

