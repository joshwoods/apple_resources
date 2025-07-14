

- Core Media I/O
- CMIOExtensionStreamProperties
-  sinkBufferUnderrunCount 

Instance Property

# sinkBufferUnderrunCount

The buffer underrun count.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var sinkBufferUnderrunCount: Int? { get set }
```

## Discussion

This value is a number the system increments whenever you’re not servicing buffers fast enough.

This property translates to the kCMIOStreamPropertyOutputBufferUnderrunCount property.

## See Also

### Configuring Sink Properties

var sinkBufferQueueSize: Int?

The buffer queue size.

var sinkBuffersRequiredForStartup: Int?

The number of buffers the stream requires for startup.

var sinkEndOfData: Int?

A value that indicates whether the stream has reached its end.

