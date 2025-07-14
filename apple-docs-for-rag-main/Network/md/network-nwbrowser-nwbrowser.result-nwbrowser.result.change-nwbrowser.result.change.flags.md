

- Network
- NWBrowser
- NWBrowser.Result
- NWBrowser.Result.Change
-  NWBrowser.Result.Change.Flags 

Structure

# NWBrowser.Result.Change.Flags

Flags providing details about a change in a discovered service.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Flags
```

## Topics

### Change Flags

static let identical: NWBrowser.Result.Change.Flags

The results are identical.

static let interfaceAdded: NWBrowser.Result.Change.Flags

The service was discovered over a new interface.

static let interfaceRemoved: NWBrowser.Result.Change.Flags

The service was no longer discovered over a certain interface.

static let metadataChanged: NWBrowser.Result.Change.Flags

The service’s associated metadata changed.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Inspecting Change Types

case identical

No change was detected for the result.

case added(NWBrowser.Result)

A new result was discovered.

case removed(NWBrowser.Result)

A previously discovered result was removed.

case changed(old: NWBrowser.Result, new: NWBrowser.Result, flags: NWBrowser.Result.Change.Flags)

A result changed properties but was not removed.

