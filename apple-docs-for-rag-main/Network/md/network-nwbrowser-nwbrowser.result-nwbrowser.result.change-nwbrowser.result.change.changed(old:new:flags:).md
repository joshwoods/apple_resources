

- Network
- NWBrowser
- NWBrowser.Result
- NWBrowser.Result.Change
-  NWBrowser.Result.Change.changed(old:new:flags:) 

Case

# NWBrowser.Result.Change.changed(old:new:flags:)

A result changed properties but was not removed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case changed(
    old: NWBrowser.Result,
    new: NWBrowser.Result,
    flags: NWBrowser.Result.Change.Flags
)
```

## See Also

### Inspecting Change Types

case identical

No change was detected for the result.

case added(NWBrowser.Result)

A new result was discovered.

case removed(NWBrowser.Result)

A previously discovered result was removed.

struct Flags

Flags providing details about a change in a discovered service.

