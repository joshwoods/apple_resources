

- AVFoundation
- AVAsyncProperty
- AVAsyncProperty.Status
-  AVAsyncProperty.Status.loaded(\_:) 

Case

# AVAsyncProperty.Status.loaded(\_:)

A property value is ready to use.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case loaded(Value)
```

## Parameters 

`value`  

A value for the property.

## See Also

### Status Values

case notYetLoaded

The system hasn’t loaded a property value.

case loading

The system is loading the property.

case failed(NSError)

A property value fails to load.

