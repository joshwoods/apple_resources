

- Finder Sync
- FIFinderSyncController
-  setTagData(\_:forItemWith:completion:) 

Instance Method

# setTagData(\_:forItemWith:completion:)

macOS 10.10+

``` source
func setTagData(
    _ tagData: Data?,
    forItemWith itemURL: URL,
    completion: @escaping (any Error) -> Void
)
```

``` source
func setTagData(
    _ tagData: Data?,
    forItemWith itemURL: URL
) async -> any Error
```

## Overview

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

