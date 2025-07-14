

- Core Media I/O
- CMIOExtensionStreamProperties
-  sinkEndOfData 

Instance Property

# sinkEndOfData

A value that indicates whether the stream has reached its end.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var sinkEndOfData: Int? { get set }
```

## Discussion

A value of `1` indicates that the stream has reached the end, and a value of `0` indicates that more data is available. This property translates to the kCMIOStreamPropertyEndOfData property.

## See Also

### Configuring Sink Properties

var sinkBufferQueueSize: Int?

The buffer queue size.

var sinkBuffersRequiredForStartup: Int?

The number of buffers the stream requires for startup.

var sinkBufferUnderrunCount: Int?

The buffer underrun count.

