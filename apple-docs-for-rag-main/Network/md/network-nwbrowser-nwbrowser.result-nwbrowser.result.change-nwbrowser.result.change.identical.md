

- Network
- NWBrowser
- NWBrowser.Result
- NWBrowser.Result.Change
-  NWBrowser.Result.Change.identical 

Case

# NWBrowser.Result.Change.identical

No change was detected for the result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case identical
```

## See Also

### Inspecting Change Types

case added(NWBrowser.Result)

A new result was discovered.

case removed(NWBrowser.Result)

A previously discovered result was removed.

case changed(old: NWBrowser.Result, new: NWBrowser.Result, flags: NWBrowser.Result.Change.Flags)

A result changed properties but was not removed.

struct Flags

Flags providing details about a change in a discovered service.

