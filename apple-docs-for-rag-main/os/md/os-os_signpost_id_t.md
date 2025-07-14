

- os
-  os_signpost_id_t 

Type Alias

# os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias os_signpost_id_t = UInt64
```

## Discussion

Multiple intervals with matching log objects and interval names can be in-flight simultaneously. In order for data-processing tools to correctly match the beginning and end of an interval, you need to identify each interval with a unique signpost identifier. Use the first strategy in the list below that matches your use case:

- If you can guarantee that intervals with the same log and name can never overlap in time, specify OS_SIGNPOST_ID_EXCLUSIVE as the signpost ID.

- If you already have your own integer data that can uniquely identify each instance of the task being measured, cast the data from a uint64_t value directly to a `os_signpost_id_t`. The value must not match one of the predefined signpost values.

- If you have a pointer that can uniquely identify begin/end pairs (such as a pointer to a data object used by the code being measured), call os_signpost_id_make_with_pointer. Don’t use this function for signposts that span process boundaries.

- Otherwise, call os_signpost_id_generate each time you create a new pair of signposts to generate a unique value for that pair.

## See Also

### Measure Events

Recording Performance Data

Add signposts to record interesting time-based events.

struct OSSignposter

An object for measuring task performance using the unified logging system.

Legacy Signpost Symbols

Migrate your code away from using these legacy symbols.

struct OSSignpostType

The different kinds of signpost.

Deprecated

