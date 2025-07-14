

- Paravirtualized Graphics
-  PGRemoveTraceRange 

Type Alias

# PGRemoveTraceRange

The block signature for a routine that removes a trace range.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGRemoveTraceRange = (OpaquePointer) -> Void
```

## Parameters 

`range`  

The trace to remove.

## See Also

### Specifying Trace Behavior

var addTraceRange: PGAddTraceRange?

A handler that the framework calls to add a trace range.

var removeTraceRange: PGRemoveTraceRange?

A handler that the framework calls to remove a trace range.

typealias PGAddTraceRange

The block signature for a routine that adds a trace range.

typealias PGTraceRangeHandler

The block signature for a routine that handles trace requests.

