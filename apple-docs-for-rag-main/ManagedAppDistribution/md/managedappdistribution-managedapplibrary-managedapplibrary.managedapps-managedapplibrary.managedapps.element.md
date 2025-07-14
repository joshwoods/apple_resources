

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
-  ManagedAppLibrary.ManagedApps.Element 

Type Alias

# ManagedAppLibrary.ManagedApps.Element

The type of element this asynchronous sequence produces.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
typealias Element = ManagedAppLibrary.ManagedApps.AsyncIterator.Element
```

## See Also

### Obtaining managed apps

struct AsyncIterator

The iterator for managed apps.

func makeAsyncIterator() -> ManagedAppLibrary.ManagedApps.AsyncIterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

