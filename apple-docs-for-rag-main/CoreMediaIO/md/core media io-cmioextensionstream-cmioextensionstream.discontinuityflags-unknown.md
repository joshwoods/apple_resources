

- Core Media I/O
- CMIOExtensionStream
- CMIOExtensionStream.DiscontinuityFlags
-  unknown 

Type Property

# unknown

A flag that indicates a stream discontinuity due to an unknown reason.

Mac Catalyst 15.4+macOS 12.3+

``` source
static var unknown: CMIOExtensionStream.DiscontinuityFlags { get }
```

## See Also

### Discontinuity Flags

static var time: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a time discontinuity in the stream.

static var sampleDropped: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a discontinuity in the stream due to a dropped frame.

