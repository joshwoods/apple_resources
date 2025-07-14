

- Core Media I/O
- CMIOExtensionStreamProperties
-  sinkBuffersRequiredForStartup 

Instance Property

# sinkBuffersRequiredForStartup

The number of buffers the stream requires for startup.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var sinkBuffersRequiredForStartup: Int? { get set }
```

## Discussion

This property translates to the kCMIOStreamPropertyOutputBuffersRequiredForStartup property.

## See Also

### Configuring Sink Properties

var sinkBufferQueueSize: Int?

The buffer queue size.

var sinkBufferUnderrunCount: Int?

The buffer underrun count.

var sinkEndOfData: Int?

A value that indicates whether the stream has reached its end.

