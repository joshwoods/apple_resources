

- AVFoundation
- AVCaptureSynchronizedDataCollection
-  synchronizedData(for:) 

Instance Method

# synchronizedData(for:)

Returns synchronized data captured by the specified capture output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func synchronizedData(for captureOutput: AVCaptureOutput) -> AVCaptureSynchronizedData?
```

## Parameters 

`captureOutput`  

The capture output for which to retrieve data.

## Return Value

A synchronized data object corresponding to the specified capture output.

## See Also

### Accessing Synchronized Data

var count: Int

The number of synchronized data objects in the collection.

subscript(AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns data captured by the specified capture output, using subscript syntax.

