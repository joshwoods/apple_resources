

- AVFoundation
- AVAsyncProperty
- AVAsyncProperty.Status
-  AVAsyncProperty.Status.loading 

Case

# AVAsyncProperty.Status.loading

The system is loading the property.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case loading
```

## See Also

### Status Values

case notYetLoaded

The system hasn’t loaded a property value.

case loaded(Value)

A property value is ready to use.

case failed(NSError)

A property value fails to load.

