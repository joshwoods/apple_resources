

- AVFoundation
- AVCaptureSynchronizedDataCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns data captured by the specified capture output, using subscript syntax.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
subscript(key: AVCaptureOutput) -> AVCaptureSynchronizedData? { get }
```

## Parameters 

`key`  

The capture output for which to retrieve data.

## Return Value

A synchronized data object corresponding to the specified capture output.

## Discussion

This call is equivalent to the synchronizedData(for:) method, but allows subscript syntax.

## See Also

### Accessing Synchronized Data

var count: Int

The number of synchronized data objects in the collection.

func synchronizedData(for: AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns synchronized data captured by the specified capture output.

