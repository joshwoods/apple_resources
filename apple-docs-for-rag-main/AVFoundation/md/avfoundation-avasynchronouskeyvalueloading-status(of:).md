

- AVFoundation
- AVAsynchronousKeyValueLoading
-  status(of:) 

Instance Method

# status(of:)

Returns a value that indicates the loaded status of a property.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func status(of property: AVAsyncProperty) -> AVAsyncProperty.Status
```

## Parameters 

`property`  

A property identifier with a status to check.

## Return Value

A status value.

## Mentioned in 

Loading media data asynchronously

## Discussion

A status of AVAsyncProperty.Status.loaded(_:) provides the property value, and a status of AVAsyncProperty.Status.failed(_:) provides an error that describes the failure.

