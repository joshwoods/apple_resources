

- Finder Sync
- FIFinderSyncController
-  setLastUsedDate(\_:forItemWith:completion:) 

Instance Method

# setLastUsedDate(\_:forItemWith:completion:)

macOS 10.10+

``` source
func setLastUsedDate(
    _ lastUsedDate: Date,
    forItemWith itemURL: URL,
    completion: @escaping (any Error) -> Void
)
```

``` source
func setLastUsedDate(
    _ lastUsedDate: Date,
    forItemWith itemURL: URL
) async -> any Error
```

## Overview

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

