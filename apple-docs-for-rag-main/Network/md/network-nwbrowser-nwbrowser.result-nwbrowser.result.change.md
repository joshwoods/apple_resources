

- Network
- NWBrowser
- NWBrowser.Result
-  NWBrowser.Result.Change 

Enumeration

# NWBrowser.Result.Change

Ways in which discovered services can change between specific results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Change
```

## Topics

### Inspecting Change Types

case identical

No change was detected for the result.

case added(NWBrowser.Result)

A new result was discovered.

case removed(NWBrowser.Result)

A previously discovered result was removed.

case changed(old: NWBrowser.Result, new: NWBrowser.Result, flags: NWBrowser.Result.Change.Flags)

A result changed properties but was not removed.

struct Flags

Flags providing details about a change in a discovered service.

### Calculating Result Changes

init(between: NWBrowser.Result?, NWBrowser.Result?)

Initializes a change between two results.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

