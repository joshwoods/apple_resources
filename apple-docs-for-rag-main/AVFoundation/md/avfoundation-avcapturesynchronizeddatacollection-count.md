

- AVFoundation
- AVCaptureSynchronizedDataCollection
-  count 

Instance Property

# count

The number of synchronized data objects in the collection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var count: Int { get }
```

## See Also

### Accessing Synchronized Data

func synchronizedData(for: AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns synchronized data captured by the specified capture output.

subscript(AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns data captured by the specified capture output, using subscript syntax.

