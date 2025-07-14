

- Finder Sync
- FIFinderSyncProtocol
-  values(forAttributes:forItemWith:completion:) 

Instance Method

# values(forAttributes:forItemWith:completion:)

macOS 10.10+

``` source
optional func values(
    forAttributes attributes: [URLResourceKey],
    forItemWith itemURL: URL,
    completion: @escaping ([URLResourceKey : Any], (any Error)?) -> Void
)
```

``` source
optional func values(
    forAttributes attributes: [URLResourceKey],
    forItemWith itemURL: URL
) async throws -> [URLResourceKey : Any]
```

## Overview

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func values(forAttributes attributes: [URLResourceKey], forItemWith itemURL: URL) async throws -> [URLResourceKey : Any]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

