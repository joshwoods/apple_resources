

- Core Media
-  CMBufferQueueGetTypeID() 

Function

# CMBufferQueueGetTypeID()

Returns the type identifier of buffer queue objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueGetTypeID() -> CFTypeID
```

## Return Value

CFTypeID of `CMBufferQueue` objects.

## Discussion

You can check if a `CFTypeRef` object is actually a `CMBufferQueue` by comparing CFGetTypeID(_:)(object) with CMBufferQueueGetTypeID()().

