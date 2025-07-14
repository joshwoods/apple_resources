

- Metal
- MTLBuffer
-  addDebugMarker(\_:range:) 

Instance Method

# addDebugMarker(\_:range:)

Adds a debug marker string to a specific buffer range.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOS

``` source
func addDebugMarker(
    _ marker: String,
    range: Range
)
```

## Parameters 

`marker`  

A string that identifies the marked buffer range.

`range`  

The range of bytes that you want to identify.

## See Also

### Debugging Buffers

func removeAllDebugMarkers()

Removes all debug marker strings from the buffer.

**Required**

