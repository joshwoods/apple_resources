

- Core Media I/O
- CMIOExtensionStream
- CMIOExtensionStream.DiscontinuityFlags
-  sampleDropped 

Type Property

# sampleDropped

A flag that indicates a discontinuity in the stream due to a dropped frame.

Mac Catalyst 15.4+macOS 12.3+

``` source
static var sampleDropped: CMIOExtensionStream.DiscontinuityFlags { get }
```

## See Also

### Discontinuity Flags

static var unknown: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a stream discontinuity due to an unknown reason.

static var time: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a time discontinuity in the stream.

