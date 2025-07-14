

- ShazamKit
- SHSession
-  delegate 

Instance Property

# delegate

The object that the session calls with the result of a match request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
weak var delegate: (any SHSessionDelegate)? { get set }
```

## See Also

### Reading the session properties

var catalog: SHCatalog

The catalog object containing the reference signatures and their associated metadata that the session uses to perform matches.

var results: SHSession.Results

The results as an asynchronous sequence of matches.

struct Results

An asynchronous sequence that emits updates from a session object query.

