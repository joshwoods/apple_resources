

- Foundation
- CodableConfiguration
-  init(wrappedValue:) 

Initializer

# init(wrappedValue:)

Creates a codable configuration wrapper for the given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(wrappedValue: T)
```

## Parameters 

`wrappedValue`  

The underlying value to make codable.

## Discussion

This initializer doesn’t take a `ConfigurationProvider.Type` parameter. As a result, it won’t compile unless the compiler can imply the provider type through other means, such as a generic expression like `@CodableConfiguration`.

For clarity, use this type’s other initializers, which take the configuration provider type as an explicit parameter.

## See Also

### Creating a Codable Configuration

init(wrappedValue: T, from: ConfigurationProvider.Type)

Creates a codable configuration wrapper for the given value, using the given configuration provider type.

init(wrappedValue: T, from: KeyPath&lt;AttributeScopes, ConfigurationProvider.Type>)

Creates a codable configuration wrapper for the given value, using given configuration provider type identified by key path.

