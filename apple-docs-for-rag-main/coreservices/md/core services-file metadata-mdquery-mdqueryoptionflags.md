

- Core Services
- File Metadata
- MDQuery
-  MDQueryOptionFlags 

Structure

# MDQueryOptionFlags

Specify the execution mode for a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
struct MDQueryOptionFlags
```

## Topics

### Constants

var kMDQuerySynchronous: MDQueryOptionFlags

Specifies that a query should block during the initial gather phase. The query’s run loop will run in the default mode. If this option is not specified the query function returns immediately after starting the query asynchronously.

var kMDQueryWantsUpdates: MDQueryOptionFlags

var kMDQueryAllowFSTranslation: MDQueryOptionFlags

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- Hashable
- RawRepresentable

