

- Combine
- Publishers
- Publishers.MapKeyPath2
-  Publishers.MapKeyPath2.Output 

Type Alias

# Publishers.MapKeyPath2.Output

The kind of values published by this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Output = (Output0, Output1)
```

## Discussion

This publisher produces two-element tuples, where each menber’s type matches the type of the corresponding key path’s property.

## See Also

### Declaring Publisher Topography

typealias Failure

The kind of errors this publisher might publish.

