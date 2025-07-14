

- Network
- NWBrowser
- NWBrowser.Result
- NWBrowser.Result.Change
-  NWBrowser.Result.Change.removed(\_:) 

Case

# NWBrowser.Result.Change.removed(\_:)

A previously discovered result was removed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case removed(NWBrowser.Result)
```

## See Also

### Inspecting Change Types

case identical

No change was detected for the result.

case added(NWBrowser.Result)

A new result was discovered.

case changed(old: NWBrowser.Result, new: NWBrowser.Result, flags: NWBrowser.Result.Change.Flags)

A result changed properties but was not removed.

struct Flags

Flags providing details about a change in a discovered service.

