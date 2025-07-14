

- Paravirtualized Graphics
-  PGTraceRangeHandler 

Type Alias

# PGTraceRangeHandler

The block signature for a routine that handles trace requests.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGTraceRangeHandler = (UnsafeMutablePointer) -> Void
```

## Parameters 

`dirty `  

The range of memory that the guest changed.

## Discussion

The returned range may be larger than the range that the guest wrote into. For example, if you can only determine which memory the guest accessed at virtual memory page boundaries, you’d report that the entire page changed. Where possible, coalesce writes over a period of time into a single activity notification.

## See Also

### Specifying Trace Behavior

var addTraceRange: PGAddTraceRange?

A handler that the framework calls to add a trace range.

var removeTraceRange: PGRemoveTraceRange?

A handler that the framework calls to remove a trace range.

typealias PGAddTraceRange

The block signature for a routine that adds a trace range.

typealias PGRemoveTraceRange

The block signature for a routine that removes a trace range.

