

- AVFoundation
- AVAsyncProperty
- AVAsyncProperty.Status
-  AVAsyncProperty.Status.failed(\_:) 

Case

# AVAsyncProperty.Status.failed(\_:)

A property value fails to load.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case failed(NSError)
```

## Parameters 

`error`  

An error object that describes the failure.

## See Also

### Status Values

case notYetLoaded

The system hasn’t loaded a property value.

case loading

The system is loading the property.

case loaded(Value)

A property value is ready to use.

