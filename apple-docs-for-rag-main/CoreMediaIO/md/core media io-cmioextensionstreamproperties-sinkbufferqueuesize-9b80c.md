

- Core Media I/O
- CMIOExtensionStreamProperties
-  sinkBufferQueueSize 

Instance Property

# sinkBufferQueueSize

The buffer queue size.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var sinkBufferQueueSize: Int? { get set }
```

## Discussion

This property translates to the kCMIOStreamPropertyOutputBufferQueueSize property.

## See Also

### Configuring Sink Properties

var sinkBuffersRequiredForStartup: Int?

The number of buffers the stream requires for startup.

var sinkBufferUnderrunCount: Int?

The buffer underrun count.

var sinkEndOfData: Int?

A value that indicates whether the stream has reached its end.

